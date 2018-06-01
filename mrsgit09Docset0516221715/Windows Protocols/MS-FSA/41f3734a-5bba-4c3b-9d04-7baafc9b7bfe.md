<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.1.2 Open of an Existing File</title>
        <xml>
            <mshelp:toctitle title="2.1.5.1.2 Open of an Existing File"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: Open of an Existing File"></mshelp:rltitle>
            <mshelp:keyword index="A" term="41f3734a-5bba-4c3b-9d04-7baafc9b7bfe"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="41f3734a-5bba-4c3b-9d04-7baafc9b7bfe"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: Open of an Existing File" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.1.2 Open of an Existing File</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>Files that require knowledge of extended attributes cannot
be opened by applications that do not understand extended attributes. If <b>CreateOptions.FILE_NO_EA_KNOWLEDGE</b>
is set and (<i>FileTypeToOpen</i> is DirectoryFile or (<i>FileTypeToOpen</i> is
DataFile and <i>StreamNameToOpen</i> is empty)) and <b>File.ExtendedAttributes</b>
contains an <i>ExistingEa</i> where <i>ExistingEa</i><b>.Flags.FILE_NEED_EA</b>
is set, the operation MUST be failed with STATUS_ACCESS_DENIED.</p>

<p>Pseudocode for the operation is as follows:</p>

<ul><li><p><span><span> 
</span></span>If <b>CreateOptions.FILE_OPEN_REPARSE_POINT</b> is not set and <b>File.ReparsePointTag</b>
is not empty, then the operation MUST be failed with <b>Status</b> set to
STATUS_REPARSE and <b>ReparsePointData</b> set to <b>File.ReparsePointData</b>.</p>

</li><li><p><span><span> 
</span></span>If <i>FileTypeToOpen</i> is DirectoryFile:</p>

<ul><li><p><span><span>  </span></span>If <b>CreateDisposition</b>
is FILE_OPEN or FILE_OPEN_IF then:</p>

<ul><li><p><span><span> 
</span></span>Perform access checks as described in section <a href="82b364ce-6d7b-422f-8d88-4db32eea809a.md">2.1.5.1.2.1</a>. If this fails
with STATUS_SHARING_VIOLATION:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains HANDLE_CACHING, the object store MUST check for an oplock break
according to the algorithm in section <a href="306239fb-cb60-49fe-b293-df4d1a5f757a.md">2.1.4.12</a>, with input
values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN_BREAK_H&quot;</p>

</li></ul></li><li><p><span><span> 
</span></span>Perform access checks as described in section 2.1.5.1.2.1. If
this fails, the request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf this fails with any other status code:</p>

<ul><li><p><span><span> 
</span></span>The request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Perform sharing access checks as described in section <a href="8c0e3f4f-0729-49f4-a14d-7f7add593819.md">2.1.5.1.2.2</a>. If this fails
with STATUS_SHARING_VIOLATION:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains HANDLE_CACHING, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li></ul></li><li><p><span><span> 
</span></span>Perform sharing access checks as described in section
2.1.5.1.2.2. If this fails, the request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf this fails with any other status code:</p>

<ul><li><p><span><span> 
</span></span>The request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.OpenList</b> is empty, <b>Open.SharingMode</b>
does not contain FILE_SHARE_READ, and <b><i>AccessCheck</i></b>(<b>SecurityContext</b>,
File.SecurityDescriptor, FILE_GENERIC_WRITE) returns FALSE:</p>

<ul><li><p><span><span> 
</span></span>If <b>CreateOptions.FILE_DISALLOW_EXCLUSIVE</b> is TRUE:<a id="Appendix_A_Target_51"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.md#Appendix_A_51" aria-label="Product behavior note 51">&lt;51&gt;</a></p>

<ul><li><p><span><span> 
</span></span>The operation MUST be failed with STATUS_ACCESS_DENIED.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>The object store MUST set <b>Open.SharingMode</b>.FILE_SHARE_READ
to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Set <b>CreateAction</b> to FILE_OPENED.</p>

</li></ul></li><li><p><span><span>  </span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>// Existing directories cannot be overwritten/superseded.</p>

</li><li><p><span><span> 
</span></span>If <b>File</b> == <b>File.Volume.RootDirectory</b>, then the
operation MUST be failed with STATUS_ACCESS_DENIED, else the operation MUST be
failed with STATUS_OBJECT_NAME_COLLISION.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>Else if <i>FileTypeToOpen</i> is DataFile:</p>

<ul><li><p><span><span>  </span></span>The
object store MUST search <b>File.StreamList</b> for a <b>Stream</b> with <b>Stream.Name</b>
matching <i>StreamNameToOpen</i>. If <b>IsCaseInsensitive</b> is TRUE, then the
search MUST be case-insensitive; otherwise it MUST be case-sensitive.</p>

</li><li><p><span><span>  </span></span>If <b>Stream</b>
was found:</p>

<ul><li><p><span><span> 
</span></span>Set <b>Open.Stream</b> to <b>Stream</b>.</p>

</li><li><p><span><span> 
</span></span>If <b>CreateDisposition</b> is FILE_CREATE, then the operation
MUST be failed with STATUS_OBJECT_NAME_COLLISION.</p>

</li><li><p><span><span> 
</span></span>If <b>CreateDisposition</b> is FILE_OPEN or FILE_OPEN_IF:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains BATCH_OPLOCK, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN&quot;</p>

</li><li><p><span><span> 
</span></span><b>OpParams</b> containing two members:</p>

<ul><li><p><span><span> 
</span></span><b>DesiredAccess</b> equal to this operation's <b>DesiredAccess</b></p>

</li><li><p><span><span> 
</span></span><b>CreateDisposition</b> equal to this operation's <b>CreateDisposition</b></p>

</li></ul></li></ul></li><li><p><span><span> 
</span></span>Perform access checks as described in section 2.1.5.1.2.1. If
this fails with STATUS_SHARING_VIOLATION:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains HANDLE_CACHING, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN_BREAK_H&quot;</p>

</li></ul></li><li><p><span><span> 
</span></span>Perform access checks as described in section 2.1.5.1.2.1. If
this fails, the request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf this fails with any other status code:</p>

<ul><li><p><span><span> 
</span></span>The request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Perform sharing access checks as described in section
2.1.5.1.2.2. If this fails with STATUS_SHARING_VIOLATION:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains HANDLE_CACHING, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN_BREAK_H&quot;</p>

</li></ul></li><li><p><span><span> 
</span></span>Perform sharing access checks as described in section 2.1.5.1.2.2.
If this fails, the request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf this fails with any other status code:</p>

<ul><li><p><span><span> 
</span></span>The request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Set <b>CreateAction</b> to FILE_OPENED.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>If <b>File.Volume.IsReadOnly</b> is TRUE, the operation MUST be
failed with STATUS_MEDIA_WRITE_PROTECTED.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains BATCH_OPLOCK, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN&quot;</p>

</li><li><p><span><span> 
</span></span><b>OpParams</b> containing two members:</p>

<ul><li><p><span><span> 
</span></span><b>DesiredAccess</b> equal to this operation's <b>DesiredAccess</b></p>

</li><li><p><span><span> 
</span></span><b>CreateDisposition</b> equal to this operation's <b>CreateDisposition</b></p>

</li></ul></li></ul></li><li><p><span><span> 
</span></span>If <b>Stream.Name</b> is empty:</p>

<ul><li><p><span><span> 
</span></span>If <b>File.FileAttributes</b>.FILE_ATTRIBUTE_HIDDEN is TRUE and <b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_HIDDEN
is FALSE, then the operation MUST be failed with STATUS_ACCESS_DENIED.</p>

</li><li><p><span><span> 
</span></span>If <b>File.FileAttributes</b>.FILE_ATTRIBUTE_SYSTEM is TRUE and <b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_SYSTEM
is FALSE, then the operation MUST be failed with STATUS_ACCESS_DENIED.</p>

</li><li><p><span><span> 
</span></span>Set <b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_ARCHIVE to TRUE.</p>

</li><li><p><span><span> 
</span></span>Set <b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_NORMAL to FALSE.</p>

</li><li><p><span><span> 
</span></span>Set <b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_NOT_CONTENT_INDEXED
to FALSE.</p>

</li><li><p><span><span> 
</span></span>If <b>File.FileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED is TRUE,
then set <b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED to TRUE.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.HasRestoreAccess</b> is TRUE, then the object store
MUST set <b>Open.GrantedAccess</b>.FILE_WRITE_EA to TRUE. Otherwise, the object
store MUST set <b>Open.RemainingDesiredAccess</b>.FILE_WRITE_EA to TRUE.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.HasRestoreAccess</b> is TRUE, then the object store
MUST set <b>Open.GrantedAccess</b>.FILE_WRITE_ATTRIBUTES to TRUE. Otherwise,
the object store MUST set <b>Open.RemainingDesiredAccess</b>.FILE_WRITE_ATTRIBUTES
to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>CreateDisposition</b> is FILE_SUPERSEDE:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.HasRestoreAccess</b> is TRUE, then the object store
MUST set <b>Open.GrantedAccess</b>.DELETE to TRUE. Otherwise, the object store
MUST set <b>Open.RemainingDesiredAccess</b>.DELETE to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.HasRestoreAccess</b> is TRUE, then the object store
MUST set <b>Open.GrantedAccess</b>.FILE_WRITE_DATA to TRUE. Otherwise, the
object store MUST set <b>Open.RemainingDesiredAccess</b>.FILE_WRITE_DATA to
TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span><b>Open.RemainingDesiredAccess</b> &amp;= ~<b>Open.GrantedAccess</b></p>

</li><li><p><span><span> 
</span></span>Perform access checks as described in section 2.1.5.1.2.1. If
this fails with STATUS_SHARING_VIOLATION:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains HANDLE_CACHING, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

</li><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN_BREAK_H&quot;</p>

</li></ul><ul><li><p><span><span> 
</span></span>Perform access checks as described in section 2.1.5.1.2.1. If
this fails, the request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf this fails with any other status code:</p>

<ul><li><p><span><span> 
</span></span>The request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Perform sharing access checks as described in section
2.1.5.1.2.2. If this fails with STATUS_SHARING_VIOLATION:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.Oplock</b> is not empty and <b>Open.Stream.Oplock.State</b>
contains HANDLE_CACHING, the object store MUST check for an oplock break
according to the algorithm in section 2.1.4.12, with input values as follows:</p>

<ul><li><p><span><span> 
</span></span><b>Open</b> equal to this operation's <b>Open</b></p>

</li><li><p><span><span> 
</span></span><b>Oplock</b> equal to <b>Open.Stream.Oplock</b></p>

</li><li><p><span><span> 
</span></span><b>Operation</b> equal to &quot;OPEN_BREAK_H&quot;</p>

</li></ul></li><li><p><span><span> 
</span></span>Perform sharing access checks as described in section
2.1.5.1.2.2. If this fails, the request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf this fails with any other status code:</p>

<ul><li><p><span><span> 
</span></span>The request MUST be failed with the same status.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Note that the file has been modified as specified in section <a href="75cdaba1-4401-4c53-b09c-69ba6cd50ce6.md">2.1.4.17</a> with <b>Open</b>
equal to <b>Open</b>.</p>

</li><li><p><span><span> 
</span></span>If <b>CreateDisposition</b> is FILE_SUPERSEDE, the object store
MUST set <b>CreateAction</b> to FILE_SUPERSEDED; otherwise, it MUST set <b>CreateAction</b>
to FILE_OVERWRITTEN.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul></li><li><p><span><span>  </span></span>Else:
// <b>Stream</b> not found.</p>

<ul><li><p><span><span> 
</span></span>If <b>CreateDisposition</b> is FILE_OPEN or FILE_OVERWRITE, the
operation MUST be failed with STATUS_OBJECT_NAME_NOT_FOUND.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.GrantedAccess</b>.FILE_WRITE_DATA is not set and <b>Open.RemainingDesiredAccess</b>.FILE_WRITE_DATA
is not set:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.HasRestoreAccess</b> is TRUE, then the object store
MUST set <b>Open.GrantedAccess</b>.FILE_WRITE_DATA to TRUE; otherwise, the
object store MUST set <b>Open.RemainingDesiredAccess</b>.FILE_WRITE_DATA to
TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Perform access checks as described in section 2.1.5.1.2.1. If
this fails, the request MUST be failed with the same status.</p>

</li><li><p><span><span> 
</span></span>If <b>File.Volume.IsReadOnly</b> is TRUE, the operation MUST be
failed with STATUS_MEDIA_WRITE_PROTECTED.</p>

</li><li><p><span><span> 
</span></span>Update <b>File.LastChangeTime</b> to the current time.</p>

</li><li><p><span><span> 
</span></span>Set <b>File.FileAttributes</b>.FILE_ATTRIBUTE_ARCHIVE to TRUE.</p>

</li><li><p><span><span> 
</span></span>Build a new <b>Stream</b> object with all fields initially set to
zero.</p>

</li><li><p><span><span> 
</span></span>Set <b>Stream.StreamType</b> to DataStream.</p>

</li><li><p><span><span> 
</span></span>Set <b>Stream.Name</b> to <i>StreamNameToOpen</i>.</p>

</li><li><p><span><span> 
</span></span>Set <b>Stream.File</b> to <b>File</b>.</p>

</li><li><p><span><span> 
</span></span>Add <b>Stream</b> to <b>File.StreamList</b>.</p>

</li><li><p><span><span> 
</span></span>Set <b>Open.Stream</b> to <b>Stream</b>.</p>

</li><li><p><span><span> 
</span></span>Set <b>CreateAction</b> to FILE_CREATED.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:  // <i>FileTypeToOpen</i> is ViewIndexFile</p>

<ul><li><p><span><span>  </span></span>//
Note that when <i>FileTypeToOpen</i> is ViewIndexFile, the stream always exists
in the file </p>

</li><li><p><span><span>  </span></span>// <b>Open.Stream.StreamType</b>
is ViewIndexStream.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If the object store implements encryption:</p>

<ul><li><p><span><span>  </span></span>If
(<b>CreateAction</b> is FILE_OVERWRITTEN or FILE_SUPERSEDED) and (<b>Stream.Name</b>
is empty) and (<b>DesiredFileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED is TRUE)
and (<b>File.FileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED is FALSE), then:</p>

<ul><li><p><span><span> 
</span></span>If <b>File.OpenList</b> is non-empty, then the operation MUST be
failed with STATUS_SHARING_VIOLATION.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>CreateAction</b> is one of FILE_OVERWRITTEN or
FILE_SUPERSEDED, then:</p>

<ul><li><p><span><span>  </span></span>If <b>Stream.Name</b>
is empty:</p>

<ul><li><p><span><span> 
</span></span>Set <b>File.FileAttributes</b> to <b>DesiredFileAttributes</b>.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If the object store implements encryption and <b>File.FileAttributes.FILE_ATTRIBUTE_ENCRYPTED</b>
is TRUE:</p>

<ul><li><p><span><span>  </span></span>If <b>CreateAction</b>
is FILE_OPENED:</p>

<ul><li><p><span><span> 
</span></span>If <b>Stream.IsEncrypted</b> is TRUE:</p>

<ul><li><p><span><span> 
</span></span>If <b>UserCertificate</b> is empty, the operation MUST be failed
with STATUS_CS_ENCRYPTION_EXISTING_ENCRYPTED_FILE.</p>

</li><li><p><span><span> 
</span></span>If <b>UserCertificate</b> is not in <b>File.UserCertificateList</b>,
the operation MUST be failed with STATUS_ACCESS_DENIED.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul></li><li><p><span><span>  </span></span>Else: 
// we are creating, overwriting, or superseding a stream</p>

<ul><li><p><span><span> 
</span></span>If <b>UserCertificate</b> is empty, the operation MUST be failed
with STATUS_CS_ENCRYPTION_NEW_ENCRYPTED_FILE.</p>

</li><li><p><span><span> 
</span></span>If <b>Stream.Name</b> is empty:</p>

<ul><li><p><span><span> 
</span></span>If <b>File.UserCertificateList</b> is empty, insert <b>UserCertificate</b>
into <b>File.UserCertificateList</b>.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>If <b>UserCertificate</b> is not in <b>File.UserCertificateList</b>,
the operation MUST be failed with STATUS_ACCESS_DENIED.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>File.FileType</b> is DataFile, set <b>Stream.IsEncrypted</b>
to TRUE.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>CreateAction</b> is one of FILE_CREATED, FILE_OVERWRITTEN
or FILE_SUPERSEDED, then:</p>

<ul><li><p><span><span>  </span></span>The
object store MUST set <i>FilterMatch</i> to a set of flags capturing
modifications to the existing file's persistent attributes performed during the
Open operation.</p>

</li><li><p><span><span>  </span></span>Send
directory change notification as specified in section <a href="7f757efa-ba81-4c0e-a4c7-d11d7beed109.md">2.1.4.1</a>, with <b>Volume</b>
equal to <b>File.Volume</b>, <b>Action</b> equal to FILE_ACTION_MODIFIED, <b>FilterMatch</b>
equal to <i>FilterMatch</i>, and <b>FileName</b> equal to <b>Open.FileName</b>.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>CreateAction</b> is FILE_CREATED, then the object store
MUST insert <b>Stream</b> into <b>File.StreamList</b>.</p>

</li><li><p><span><span> 
</span></span>If <b>File</b> is not in <b>File.Volume.OpenFileList</b>, the
object store MUST insert it.</p>

</li><li><p><span><span> 
</span></span>The object store MUST insert <b>Open</b> into <b>File.OpenList</b>.</p>

</li><li><p><span><span> 
</span></span>If Stream.Name is not empty:</p>

<ul><li><p><span><span>  </span></span>If <b>CreateAction</b>
is FILE_CREATED:</p>

<ul><li><p><span><span> 
</span></span>Send directory change notification as specified in section
2.1.4.1, with <b>Volume</b> equal to <b>File.Volume</b>, <b>Action</b> equal to
FILE_ACTION_ADDED_STREAM, <i>FilterMatch</i> equal to
FILE_NOTIFY_CHANGED_STREAM_NAME, and <b>FileName</b> equal to <b>Open.FileName</b>
+ &quot;:&quot; + <b>Stream.Name</b>.</p>

</li></ul></li><li><p><span><span>  </span></span>If <b>CreateAction</b>
is one of FILE_OVERWRITTEN or FILE_SUPERSEDED:</p>

<ul><li><p><span><span> 
</span></span>Send directory change notification as specified in section
2.1.4.1, with <b>Volume</b> equal to <b>File.Volume</b>, <b>Action</b> equal to
FILE_ACTION_MODIFIED_STREAM, <i>FilterMatch</i> equal to
(FILE_NOTIFY_CHANGE_STREAM_SIZE | FILE_NOTIFY_CHANGE_STREAM_WRITE), and <b>FileName</b>
equal to <b>Open.FileName</b> + &quot;:&quot; + <b>Stream.Name</b>.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>The object store SHOULD update the duplicated information as
specified in section <a href="7e375703-5641-48f3-b844-c2ef1ee70461.md">2.1.4.18</a>
with <b>Link</b> equal to <b>Open.Link</b>.</p>

</li><li><p><span><span> 
</span></span>The object store MUST return:</p>

<ul><li><p><span><span>  </span></span><b>Status</b>
set to STATUS_SUCCESS.</p>

</li><li><p><span><span>  </span></span><b>CreateAction</b>
set to FILE_OPENED.</p>

</li><li><p><span><span>  </span></span>The
<b>Open</b> object created previously.</p>

</li></ul></li></ul>
                </div>
            </div>
        </div>
    </body>
</html>