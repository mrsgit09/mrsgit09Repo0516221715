<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.1 Server Requests an Open of a File</title>
        <xml>
            <mshelp:toctitle title="2.1.5.1 Server Requests an Open of a File"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: Server Requests an Open of a File"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8ada5fbe-db4e-49fd-aef6-20d54b748e40"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8ada5fbe-db4e-49fd-aef6-20d54b748e40"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: Server Requests an Open of a File" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.1 Server Requests an Open of a File</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The server provides:</p>

<ul><li><p><span><span> 
</span></span><b>RootOpen:</b> An <b>Open</b> to the root of the share.</p>

</li><li><p><span><span> 
</span></span><b>PathName:</b> A <a href="682f0f59-385c-4351-b81a-3b234f53db03.md#gt_c305d0ab-8b94-461a-bd76-13b40cb8c4d8">Unicode</a> path relative to <b>RootOpen</b>
for the file to be opened in the format specified in <mshelp:link keywords="efbfe127-73ad-4140-9967-ec6500e66d5e" tabindex="0">[MS-FSCC]</mshelp:link>
section <mshelp:link keywords="ffb795f3-027d-4a3c-997d-3085f2332f6f" tabindex="0">2.1.5</mshelp:link>.</p>

</li><li><p><span><span> 
</span></span><b>SecurityContext:</b> The <b>SecurityContext</b> of the user
performing the open.</p>

</li><li><p><span><span> 
</span></span><b>DesiredAccess:</b> A bitmask indicating requested access for
the open, as specified in <mshelp:link keywords="5606ad47-5ee0-437a-817e-70c366052962" tabindex="0">[MS-SMB2]</mshelp:link>
section <mshelp:link keywords="b3af3aaf-9271-4419-b326-eba0341df7d2" tabindex="0">2.2.13.1</mshelp:link>.</p>

</li><li><p><span><span> 
</span></span><b>ShareAccess:</b> A bitmask indicating sharing access for the
open, as specified in [MS-SMB2] section <mshelp:link keywords="e8fb45c1-a03d-44ca-b7ae-47385cfd7997" tabindex="0">2.2.13</mshelp:link>.</p>

</li><li><p><span><span> 
</span></span><b>CreateOptions:</b> A bitmask of options for the open, as
specified in [MS-SMB2] section 2.2.13.</p>

</li><li><p><span><span> 
</span></span><b>CreateDisposition:</b> The requested disposition for the open,
as specified in [MS-SMB2] section 2.2.13.</p>

</li><li><p><span><span> 
</span></span><b>DesiredFileAttributes:</b> A bitmask of requested file
attributes for the open, as specified in [MS-SMB2] section 2.2.13.</p>

</li><li><p><span><span> 
</span></span><b>IsCaseInsensitive:</b> A Boolean value. TRUE indicates that
string comparisons performed in the context of this Open are case-insensitive;
otherwise, they are case-sensitive.</p>

</li><li><p><span><span> 
</span></span><b>TargetOplockKey:</b> A <a href="682f0f59-385c-4351-b81a-3b234f53db03.md#gt_f49694cc-c350-462d-ab8e-816f0103c6c1">GUID</a> value. This value
could be empty.</p>

</li><li><p><span><span> 
</span></span><b>UserCertificate:</b> An ENCRYPTION_CERTIFICATE structure as
specified in <mshelp:link keywords="08796ba8-01c8-4872-9221-1000ec2eff31" tabindex="0">[MS-EFSR]</mshelp:link>
section <mshelp:link keywords="6e0da5b4-1d90-45b1-82df-8c64cf6bbc9e" tabindex="0">2.2.8</mshelp:link>
and used when opening an encrypted stream. This value could be empty.</p>

</li></ul><p>On completion, the object store MUST return:</p>

<ul><li><p><span><span> 
</span></span><b>Status:</b> An NTSTATUS code that specifies the result.</p>

</li></ul><p>On success it MUST also return:</p>

<ul><li><p><span><span> 
</span></span><b>CreateAction:</b> A code defining the action taken by the open
operation, as specified in [MS-SMB2] section <mshelp:link keywords="d166aa9e-0b53-410e-b35e-3933d8131927" tabindex="0">2.2.14</mshelp:link>
for the <b>CreateAction</b> field.</p>

</li><li><p><span><span> 
</span></span><b>Open:</b> The newly created <b>Open</b>.</p>

</li></ul><p>On STATUS_REPARSE or STATUS_STOPPED_ON_SYMLINK it MUST also
return:</p>

<ul><li><p><span><span> 
</span></span><b>ReparseData:</b> The <a href="682f0f59-385c-4351-b81a-3b234f53db03.md#gt_4fed0b53-5fc8-4818-886f-93d87f3035e1">reparse point</a> data
associated with an existing file, in the format described in [MS-FSCC] section <mshelp:link keywords="e57148b1-300b-4d1e-8f67-091de2de815e" tabindex="0">2.1.2</mshelp:link>.
The application MAY retry the open operation with a different <b>PathName</b>
parameter constructed using <b>ReparseData</b>.</p>

</li></ul><p>Pseudocode for the operation is as follows:</p>

<ul><li><p><span><span> 
</span></span>Phase 1 -- Parameter Validation:</p>

</li><li><p><span><span> 
</span></span>Set <i>ValidDirectoryCreateOptions</i> = (FILE_DIRECTORY_FILE |
FILE_SYNCHRONOUS_IO_ALERT | FILE_SYNCHRONOUS_IO_NONALERT | FILE_WRITE_THROUGH |
FILE_OPEN_REMOTE_INSTANCE | FILE_COMPLETE_IF_OPLOCKED |
FILE_OPEN_FOR_BACKUP_INTENT | FILE_DELETE_ON_CLOSE | FILE_OPEN_FOR_FREE_SPACE_QUERY
| FILE_OPEN_BY_FILE_ID | FILE_NO_COMPRESSION | FILE_OPEN_REPARSE_POINT |
FILE_OPEN_REQUIRING_OPLOCK).</p>

</li><li><p><span><span> 
</span></span>The operation MUST be failed with STATUS_INVALID_PARAMETER under
any of the following conditions:</p>

<ul><li><p><span><span>  </span></span>If <b>RootOpen.File.FileType</b>
is DataFile.</p>

</li><li><p><span><span>  </span></span>If <b>ShareAccess</b>,
<b>CreateOptions</b>, <b>CreateDisposition</b>, or <b>FileAttributes</b> are
not valid values for a file object as specified in [MS-SMB2] section 2.2.13.</p>

</li><li><p><span><span>  </span></span>If
(<b>CreateOptions.FILE_SYNCHRONOUS_IO_ALERT</b> || <b>Create.FILE_SYNCHRONOUS_IO_NONALERT</b>)
&amp;&amp; !<b>DesiredAccess.SYNCHRONIZE</b>.</p>

</li><li><p><span><span>  </span></span>If <b>CreateOptions.FILE_DELETE_ON_CLOSE</b>
&amp;&amp; !<b>DesiredAccess.DELETE</b>.</p>

</li><li><p><span><span>  </span></span>If <b>CreateOptions.FILE_SYNCHRONOUS_IO_ALERT</b>
&amp;&amp; <b>Create.FILE_SYNCHRONOUS_IO_NONALERT</b>.</p>

</li><li><p><span><span>  </span></span>If <b>CreateOptions.FILE_DIRECTORY_FILE</b>
is TRUE &amp;&amp; <b>CreateOptions.FILE_NON_DIRECTORY_FILE</b> is FALSE
&amp;&amp; ((<b>CreateOptions</b> &amp; ~ <i>ValidDirectoryCreateOptions</i>)
|| (<b>CreateDisposition</b> != FILE_CREATE &amp;&amp; <b>CreateDisposition</b>
!= FILE_OPEN &amp;&amp; <b>CreateDisposition</b> != FILE_OPEN_IF)).</p>

</li><li><p><span><span>  </span></span>If <b>CreateOptions.FILE_COMPLETE_IF_OPLOCKED</b>
&amp;&amp; <b>CreateOptions.FILE_RESERVE_OPFILTER</b>.</p>

</li><li><p><span><span>  </span></span>If <b>CreateOptions.FILE_NO_INTERMEDIATE_BUFFERING</b>
&amp;&amp; <b>DesiredAccess.FILE_APPEND_DATA</b>.</p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>DesiredAccess</b> is zero, or if any of the bits in the
mask 0x0CE0FE00 are set, the operation MUST be failed with
STATUS_ACCESS_DENIED.</p>

</li><li><p><span><span> 
</span></span>If <b>CreateOptions.FILE_DIRECTORY_FILE</b> &amp;&amp; <b>CreateOptions.FILE_NON_DIRECTORY_FILE</b>,
the operation MUST be failed with STATUS_INVALID_PARAMETER.</p>

</li><li><p><span><span> 
</span></span>The operation MUST be failed with STATUS_OBJECT_NAME_INVALID
under any of the following conditions:</p>

<ul><li><p><span><span>  </span></span>If <b>PathName</b>
is not valid as specified in [MS-FSCC] section 2.1.5.</p>

</li><li><p><span><span>  </span></span>If <b>PathName</b>
contains a trailing backslash and <b>CreateOptions.FILE_NON_DIRECTORY_FILE</b>
is TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>DesiredFileAttributes.FILE_ATTRIBUTE_ENCRYPTED</b> is
specified, then the object store MUST set <b>CreateOptions.FILE_NO_COMPRESSION</b>.</p>

</li><li><p><span><span> 
</span></span>Phase 2 -- Volume State:</p>

</li><li><p><span><span> 
</span></span>If <b>RootOpen.File.Volume.IsReadOnly</b> &amp;&amp; (<b>CreateDisposition</b>
== FILE_CREATE || <b>CreateDisposition</b> == FILE_SUPERSEDE || <b>CreateDisposition</b>
== OVERWRITE || <b>CreateDisposition</b> == OVERWRITE_IF) then the operation
MUST be failed with STATUS_MEDIA_WRITE_PROTECTED.</p>

</li><li><p><span><span> 
</span></span>Phase 3 -- Initialization of <b>Open</b> Object:</p>

</li><li><p><span><span> 
</span></span>The object store MUST build a new <b>Open</b> object with fields
initialized as follows:</p>

<ul><li><p><span><span>  </span></span><b>Open.RootOpen</b>
set to <b>RootOpen.</b></p>

</li><li><p><span><span>  </span></span><b>Open.FileName</b>
formed by concatenating <b>RootOpen.FileName</b> + &quot;\&quot; + <b>FileName</b>,
stripping any redundant backslashes and trailing backslashes.</p>

</li><li><p><span><span>  </span></span><b>Open.RemainingDesiredAccess</b>
set to <b>DesiredAccess</b>.</p>

</li><li><p><span><span>  </span></span><b>Open.SharingMode</b>
set to <b>ShareAccess</b>.</p>

</li><li><p><span><span>  </span></span><b>Open.Mode</b>
set to (<b>CreateOptions</b> &amp; (FILE_WRITE_THROUGH | FILE_SEQUENTIAL_ONLY |
FILE_NO_INTERMEDIATE_BUFFERING | FILE_SYNCHRONOUS_IO_ALERT |
FILE_SYNCHRONOUS_IO_NONALERT | FILE_DELETE_ON_CLOSE)).</p>

</li><li><p><span><span>  </span></span><b>Open.IsCaseInsensitive</b>
set to <b>IsCaseInsensitive</b>.</p>

</li><li><p><span><span>  </span></span><b>Open.HasBackupAccess</b>
set to TRUE if <b>SecurityContext.PrivilegeSet</b> contains
&quot;SeBackupPrivilege&quot;.</p>

</li><li><p><span><span>  </span></span><b>Open.HasRestoreAccess</b>
set to TRUE if <b>SecurityContext.PrivilegeSet</b> contains
&quot;SeRestorePrivilege&quot;.</p>

</li><li><p><span><span>  </span></span><b>Open.HasCreateSymbolicLinkAccess</b>
set to TRUE if <b>SecurityContext.PrivilegeSet</b> contains
&quot;SeCreateSymbolicLinkPrivilege&quot;.</p>

</li><li><p><span><span>  </span></span><b>Open.HasManageVolumeAccess</b>
set to TRUE if <b>SecurityContext.PrivilegeSet</b> contains
&quot;SeManageVolumePrivilege&quot;.</p>

</li><li><p><span><span>  </span></span><b>Open.IsAdministrator</b>
set to TRUE if <b>SecurityContext.SIDs</b> contains the well-known SID
BUILTIN_ADMINISTRATORS as defined in <mshelp:link keywords="cca27429-5689-4a16-b2b4-9325d93e4ba2" tabindex="0">[MS-DTYP]</mshelp:link>
section <mshelp:link keywords="81d92bba-d22b-4a8c-908a-554ab29148ab" tabindex="0">2.4.2.4</mshelp:link>.</p>

</li><li><p><span><span>  </span></span><b>Open.TargetOplockKey</b>
set to <b>TargetOplockKey</b>.</p>

</li><li><p><span><span>  </span></span><b>Open.LastQuotaId</b>
set to -1.</p>

</li><li><p><span><span>  </span></span>All
other fields set to zero.</p>

</li></ul></li><li><p><span><span> 
</span></span>Phase 4 -- Check for <a href="682f0f59-385c-4351-b81a-3b234f53db03.md#gt_f0ec1e1a-3f20-40f1-8b67-b892ff3e4b72">backup</a>/<a href="682f0f59-385c-4351-b81a-3b234f53db03.md#gt_43eabdaa-8fc0-48ac-a23e-2cd92a2fa481">restore</a> intent</p>

</li><li><p><span><span> 
</span></span>If <b>CreateOptions.FILE_OPEN_FOR_BACKUP_INTENT</b> is set and (<b>CreateDisposition</b>
== FILE_OPEN || <b>CreateDisposition</b> == FILE_OPEN_IF || <b>CreateDisposition</b>
== FILE_OVERWRITE_IF) and <b>Open.HasBackupAccess</b> is TRUE, then the object
store SHOULD grant backup access as shown in the following pseudocode:</p>

<ul><li><p><span><span>  </span></span><i>BackupAccess</i>
= (READ_CONTROL | ACCESS_SYSTEM_SECURITY | FILE_GENERIC_READ | FILE_TRAVERSE)</p>

</li><li><p><span><span>  </span></span>If <b>Open.RemainingDesiredAccess.MAXIMUM_ALLOWED</b>
is set then:</p>

<ul><li><p><span><span> 
</span></span><b>Open.GrantedAccess</b> |= <i>BackupAccess</i></p>

</li></ul></li><li><p><span><span>  </span></span>Else:</p>

<ul><li><p><span><span> 
</span></span><b>Open.GrantedAccess</b> |= (<b>Open.RemainingDesiredAccess</b>
&amp; <i>BackupAccess</i>)</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li><li><p><span><span>  </span></span><b>Open.RemainingDesiredAccess</b>
&amp;= ~<b>Open.GrantedAccess</b></p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>CreateOptions.FILE_OPEN_FOR_BACKUP_INTENT</b> is set and <b>Open.HasRestoreAccess</b>
is TRUE, then the object store SHOULD grant restore access as shown in the
following pseudocode:</p>

<ul><li><p><span><span>  </span></span><i>RestoreAccess</i>
= (WRITE_DAC | WRITE_OWNER | ACCESS_SYSTEM_SECURITY | FILE_GENERIC_WRITE |
FILE_ADD_FILE | FILE_ADD_SUBDIRECTORY | DELETE)</p>

</li><li><p><span><span>  </span></span>If <b>Open.RemainingDesiredAccess.MAXIMUM_ALLOWED</b>
is set then:</p>

<ul><li><p><span><span> 
</span></span><b>Open.GrantedAccess</b> |= <i>RestoreAccess</i></p>

</li></ul></li><li><p><span><span>  </span></span>Else:</p>

<ul><li><p><span><span> 
</span></span><b>Open.GrantedAccess</b> |= (<b>Open.RemainingDesiredAccess</b>
&amp; <i>RestoreAccess</i>)</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li><li><p><span><span>  </span></span><b>Open.RemainingDesiredAccess</b>
&amp;= ~<b>Open.GrantedAccess</b></p>

</li></ul></li><li><p><span><span> 
</span></span>Phase 5 -- Parse pathname:</p>

</li><li><p><span><span> 
</span></span>The object store MUST split <b>Open.FileName</b> into pathname
components <i>PathName</i><sub>1</sub> ... <i>PathName</i><sub>n</sub>, using
the backslash (&quot;\&quot;) character as a delimiter. If any <i>PathName</i><sub>i</sub>
ends in a colon(&quot;:&quot;) character, the operation MUST be failed with
STATUS_OBJECT_NAME_INVALID. The object store MUST further split each <i>PathName</i><sub>i</sub>
into a file name component <i>FileName</i><sub>i</sub>, stream name component <i>StreamName</i><sub>i</sub>,
and stream type name component <i>StreamTypeName</i><sub>i</sub>, using the
colon (&quot;:&quot;) character as a delimiter (<i>FileName</i><sub>i</sub>:<i>StreamName</i><sub>i</sub>:<i>StreamTypeName</i><sub>i</sub>).
If <i>StreamName</i><sub>i</sub> or <i>StreamTypeName</i><sub>i</sub> is not
present in the name, the value MUST be set to an empty string.</p>

</li><li><p><span><span> 
</span></span>Phase 6 -- Location of file:</p>

</li><li><p><span><span> 
</span></span>The object store MUST search for a filename matching <b>Open.FileName</b>.
If <b>IsCaseInsensitive</b> is TRUE, then the search MUST be case-insensitive;
otherwise it MUST be case-sensitive. Pseudocode for this search is as follows:</p>

<ul><li><p><span><span>  </span></span>Set
<i>ParentFile</i> = <b>RootOpen.File</b>.</p>

</li><li><p><span><span>  </span></span>//
Examine each prefix pathname component in order.</p>

</li><li><p><span><span>  </span></span>For
i = 1 to n-1: // n is the number of pathname components, from Phase 5.</p>

<ul><li><p><span><span> 
</span></span>If <i>StreamTypeName</i><sub>i</sub> is non-empty:</p>

<ul><li><p><span><span> 
</span></span>Set <i>ComplexNameSuffix</i> = &quot;:StreamName<sub>i</sub>:<i>StreamTypeName</i><sub>i</sub>&quot;.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else if <i>StreamTypeName</i><sub>i</sub> is non-empty:</p>

<ul><li><p><span><span> 
</span></span>Set <i>ComplexNameSuffix</i> = &quot;:<i>StreamName</i><sub>i</sub>&quot;.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>Set <i>ComplexNameSuffix</i> to empty.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <i>ComplexNameSuffix</i> is non-empty and <i>ComplexNameSuffix</i>
is not equal to one of the complex name suffixes recognized by the object store<a id="Appendix_A_Target_42"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.md#Appendix_A_42" aria-label="Product behavior note 42">&lt;42&gt;</a> (using case-insensitive string
comparisons), the operation MUST be failed with STATUS_OBJECT_NAME_INVALID.</p>

</li><li><p><span><span> 
</span></span>Search <i>ParentFile</i>.<b>DirectoryList</b> for a <b>Link</b>
where <b>Link.Name</b> or <b>Link.ShortName</b> matches <i>FileName</i><sub>i</sub>.
If no such link is found, the operation MUST be failed with
STATUS_OBJECT_PATH_NOT_FOUND.</p>

</li><li><p><span><span> 
</span></span>If <b>Link.File.FileType</b> is not DirectoryFile, the operation
MUST be failed with STATUS_NOT_A_DIRECTORY.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.GrantedAccess.FILE_TRAVERSE</b> is not set and <b><i>AccessCheck</i></b>(<b>SecurityContext</b>,
<b>Link.File.SecurityDescriptor</b>, FILE_TRAVERSE) returns FALSE, the
operation MAY be failed with STATUS_ACCESS_DENIED.</p>

</li><li><p><span><span> 
</span></span>If <b>Link.IsDeleted</b>, the operation MUST be failed with
STATUS_DELETE_PENDING.</p>

</li><li><p><span><span> 
</span></span>If <b>Link.File.IsSymbolicLink</b> is TRUE, the operation MUST be
failed with <b>Status</b> set to STATUS_STOPPED_ON_SYMLINK and <b>ReparsePointData</b>
set to <b>Link.File.ReparsePointData</b>.</p>

</li><li><p><span><span> 
</span></span>Set <i>ParentFile</i> = <b>Link.File</b>.</p>

</li></ul></li><li><p><span><span>  </span></span>EndFor</p>

</li><li><p><span><span>  </span></span>//
Examine final pathname component.</p>

</li><li><p><span><span>  </span></span>Set
<i>FileNameToOpen</i> to <i>FileName</i><sub>n</sub>, <i>StreamNameToOpen</i>
to <i>StreamName</i><sub>n</sub>, and <i>StreamTypeNameToOpen</i> to <i>StreamTypeName</i><sub>n</sub>.</p>

</li><li><p><span><span>  </span></span>If <i>StreamTypeNameToOpen</i>
is non-empty and <i>StreamTypeNameToOpen</i> is not equal to one of the stream
type names recognized by the object store<a id="Appendix_A_Target_43"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.md#Appendix_A_43" aria-label="Product behavior note 43">&lt;43&gt;</a> (using
case-insensitive string comparisons), the operation MUST be failed with
STATUS_OBJECT_NAME_INVALID.</p>

</li><li><p><span><span>  </span></span>Search
<i>ParentFile</i>.<b>DirectoryList</b> for a <b>Link</b> where <b>Link.Name</b>
or <b>Link.ShortName</b> matches <i>FileNameToOpen</i>. If such a link is
found:</p>

<ul><li><p><span><span> 
</span></span>Set <b>File</b> = <b>Link.File</b>.</p>

</li><li><p><span><span> 
</span></span>Set <b>Open.File</b> to <b>File</b>.</p>

</li><li><p><span><span> 
</span></span>Set <b>Open.Link</b> to <b>Link</b>.</p>

</li></ul></li><li><p><span><span>  </span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>If (<b>CreateDisposition ==</b> FILE_OPEN || <b>CreateDisposition
==</b> FILE_OVERWRITE), the operation MUST be failed with
STATUS_OBJECT_NAME_NOT_FOUND.</p>

</li><li><p><span><span> 
</span></span>If <b>RootOpen.File.Volume.IsReadOnly</b> then the operation MUST
be failed with STATUS_MEDIA_WRITE_PROTECTED.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li><li><p><span><span>  </span></span>If <i>StreamTypeNameToOpen</i>
is non-empty and has a value other than &quot;$DATA&quot; or
&quot;$INDEX_ALLOCATION&quot;, the operation MUST be failed with
STATUS_OBJECT_NAME_INVALID.</p>

</li></ul></li><li><p><span><span> 
</span></span>Phase 7 -- Type of file to open:</p>

</li><li><p><span><span> 
</span></span>The object store MUST use the following algorithm to determine
which type of file is being opened:</p>

</li><li><p><span><span> 
</span></span>Set <i>FileTypeToOpen</i> to empty.</p>

</li><li><p><span><span> 
</span></span>If <b>RootOpen.File.Volume.IsPhysicalRoot</b> is TRUE, then set <i>FileTypeToOpen</i>
to ViewIndexFile under any of the following conditions:</p>

<ul><li><p><span><span>  </span></span>If <b>RootOpen.File.Volume.IsObjectIDsSupported</b>
is TRUE, <b>BuildRelativeName</b>(<b>Open.Link</b>, <b>Open.File.Volume.RootDirectory</b>)
is equal to &quot;\$Extend\$ObjId&quot;, <i>StreamNameToOpen</i> is equal to
&quot;$O&quot;, and <i>StreamTypeNameToOpen</i> is equal to
&quot;$INDEX_ALLOCATION&quot; (using case-insensitive string comparisons).</p>

</li><li><p><span><span>  </span></span>If <b>RootOpen.File.Volume.IsQuotasSupported</b>
is TRUE, <b>BuildRelativeName</b>(<b>Open.Link</b>, <b>Open.File.Volume.RootDirectory</b>)
is equal to &quot;\$Extend\$Quota&quot;, <i>StreamNameToOpen</i> is equal to
&quot;$O&quot; or &quot;$Q&quot;, and <i>StreamTypeNameToOpen</i> is equal to
&quot;$INDEX_ALLOCATION&quot; (using case-insensitive string comparisons).</p>

</li><li><p><span><span>  </span></span>If <b>RootOpen.File.Volume.IsReparsePointsSupported</b>
is TRUE, <b>BuildRelativeName</b>(<b>Open.Link</b>, <b>Open.File.Volume.RootDirectory</b>)
is equal to &quot;\$Extend\$Reparse&quot;, <i>StreamNameToOpen</i> is equal to
&quot;$R&quot;, and <i>StreamTypeNameToOpen</i> is equal to
&quot;$INDEX_ALLOCATION&quot; (using case-insensitive string comparisons).</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>// Note that when <i>FileTypeToOpen</i> is ViewIndexFile, the
file always exists in the object store and </p>

</li><li><p><span><span> 
</span></span>// <b>Open.File.FileType</b> is ViewIndexFile.</p>

</li><li><p><span><span> 
</span></span>If <i>FileTypeToOpen</i> is empty:</p>

<ul><li><p><span><span>  </span></span>If <i>StreamTypeNameToOpen</i>
is &quot;$INDEX_ALLOCATION&quot; and <i>StreamNameToOpen</i> has a value other
than an empty stream or &quot;$I30&quot;, the operation SHOULD<a id="Appendix_A_Target_44"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.md#Appendix_A_44" aria-label="Product behavior note 44">&lt;44&gt;</a> be failed with
STATUS_INVALID_PARAMETER.</p>

</li><li><p><span><span>  </span></span>If <b>CreateOptions.FILE_DIRECTORY_FILE</b>
is TRUE then <i>FileTypeToOpen</i> = DirectoryFile.</p>

</li><li><p><span><span>  </span></span>Else
if <b>CreateOptions.FILE_NON_DIRECTORY_FILE</b> is TRUE then <i>FileTypeToOpen</i>
= DataFile.</p>

</li><li><p><span><span>  </span></span>Else
if <i>StreamTypeNameToOpen</i> is &quot;$INDEX_ALLOCATION&quot; then <i>FileTypeToOpen</i>
= DirectoryFile.</p>

</li><li><p><span><span>  </span></span>Else
if <i>StreamTypeNameToOpen</i> is &quot;$DATA&quot; then <i>FileTypeToOpen</i>
= DataFile.</p>

</li><li><p><span><span>  </span></span>Else
if <b>Open.File</b> is not NULL and <b>Open.File.FileType</b> is DirectoryFile,
then <i>FileTypeToOpen</i> = DirectoryFile.</p>

</li><li><p><span><span>  </span></span>Else
if <b>PathName</b> contains a trailing backslash then <i>FileTypeToOpen</i> =
DirectoryFile.</p>

</li><li><p><span><span>  </span></span>Else
<i>FileTypeToOpen</i> = DataFile.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <i>FileTypeToOpen</i> is DirectoryFile and <b>Open.File</b> is
not NULL and <b>Open.File.FileType</b> is not DirectoryFile:</p>

<ul><li><p><span><span>  </span></span>If <b>CreateDisposition</b>
== FILE_CREATE then the operation MUST be failed with
STATUS_OBJECT_NAME_COLLISION, else the operation MUST be failed with
STATUS_NOT_A_DIRECTORY.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <i>FileTypeToOpen</i> is DataFile and <i>StreamNameToOpen</i>
is empty and <b>Open.File</b> is not NULL and <b>Open.File.FileType</b> is
DirectoryFile, the operation MUST be failed with STATUS_FILE_IS_A_DIRECTORY.</p>

</li><li><p><span><span> 
</span></span>Phase 8 -- Completion of open</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File</b> is NULL, the object store MUST create a new
file as described in section <a href="498a5eeb-afc9-445f-99ed-a7e4b73c648b.md">2.1.5.1.1</a>;
otherwise the object store MUST open the existing file as described in section <a href="41f3734a-5bba-4c3b-9d04-7baafc9b7bfe.md">2.1.5.1.2</a>.</p>

</li></ul>
                </div>
            </div>
        </div>
    </body>
</html>