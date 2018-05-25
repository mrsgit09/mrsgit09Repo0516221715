<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.9.27 FSCTL_SET_ENCRYPTION</title>
        <xml>
            <mshelp:toctitle title="2.1.5.9.27 FSCTL_SET_ENCRYPTION"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: FSCTL_SET_ENCRYPTION"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ad5ba3b9-ceb1-44e0-adc4-237ba533fdad"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ad5ba3b9-ceb1-44e0-adc4-237ba533fdad"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: FSCTL_SET_ENCRYPTION" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.9.27 FSCTL_SET_ENCRYPTION</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The server provides:</p>

<ul><li><p><span><span> 
</span></span><b>Open:</b> An <b>Open</b> of a DataFile or DirectoryFile.</p>

</li><li><p><span><span> 
</span></span><b>InputBuffer:</b> An array of bytes containing an
ENCRYPTION_BUFFER structure indicating the requested encryption state of the
stream or file, as specified in <mshelp:link keywords="efbfe127-73ad-4140-9967-ec6500e66d5e" tabindex="0">[MS-FSCC]</mshelp:link>
section <mshelp:link keywords="bf78ff7e-b0a4-4ba9-8825-4af43682eb0d" tabindex="0">2.3.55</mshelp:link>.</p>

</li><li><p><span><span> 
</span></span><b>InputBufferSize:</b> The number of bytes in <b>InputBuffer</b>.</p>

</li></ul><p>On completion, the object store MUST return:</p>

<ul><li><p><span><span> 
</span></span><b>Status:</b> An NTSTATUS code that specifies the result.</p>

</li></ul><p>This operation uses the following local variables:</p>

<ul><li><p><span><span> 
</span></span>Boolean value (initialized to FALSE): <i>ChangedFileEncryption</i></p>

</li></ul><p>Support for this operation is optional. If the object store
does not implement this functionality, the operation MUST be failed with
STATUS_INVALID_DEVICE_REQUEST.<a id="Appendix_A_Target_101"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.html#Appendix_A_101" aria-label="Product behavior note 101">&lt;101&gt;</a></p>

<p>Pseudocode for the operation is as follows:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.File.Volume.IsReadOnly</b> is TRUE, the operation MUST
be failed with STATUS_MEDIA_WRITE_PROTECTED.</p>

</li><li><p><span><span> 
</span></span>If <b>InputBufferSize</b> is smaller than <b><i>BlockAlign(sizeof(</i></b>ENCRYPTION_BUFFER<b><i>)</i></b>,
4<b><i>)</i></b>, the operation MUST be failed with STATUS_BUFFER_TOO_SMALL.</p>

</li><li><p><span><span> 
</span></span>The operation MUST be failed with STATUS_INVALID_PARAMETER under
any of the following conditions:</p>

<ul><li><p><span><span>  </span></span>If <b>InputBuffer.EncryptionOperation</b>
is not one of the predefined values in [MS-FSCC] section 2.3.55.</p>

</li><li><p><span><span>  </span></span>If <b>InputBuffer.EncryptionOperation</b>
== STREAM_SET_ENCRYPTION and <b>Open.Stream.IsCompressed</b> is TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>InputBuffer.EncryptionOperation</b> == FILE_SET_ENCRYPTION:</p>

<ul><li><p><span><span>  </span></span>If <b>Open.File.Attributes</b>.FILE_ATTRIBUTE_ENCRYPTED
is FALSE:</p>

<ul><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED
to TRUE.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.PendingNotifications</b>.FILE_NOTIFY_CHANGE_ATTRIBUTES
to TRUE.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <i>ChangedFileEncryption</i> to TRUE.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf <b>InputBuffer.EncryptionOperation</b> ==
FILE_CLEAR_ENCRYPTION:</p>

<ul><li><p><span><span>  </span></span>If <b>Open.File.Attributes</b>.FILE_ATTRIBUTE_ENCRYPTED
is TRUE:</p>

<ul><li><p><span><span> 
</span></span>If there exists an <i>ExistingStream</i> in <b>Open.File.StreamList</b>
such that <i>ExistingStream</i>.<b>IsEncrypted</b> is TRUE, the operation MUST
be failed with STATUS_INVALID_DEVICE_REQUEST.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED
to FALSE.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.PendingNotifications</b>.FILE_NOTIFY_CHANGE_ATTRIBUTES
to TRUE.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <i>ChangedFileEncryption</i> to TRUE.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>ElseIf <b>InputBuffer.EncryptionOperation</b> ==
STREAM_SET_ENCRYPTION:</p>

<ul><li><p><span><span>  </span></span>If <b>Open.Stream.IsEncrypted</b>
is FALSE:</p>

<ul><li><p><span><span> 
</span></span>The object store MUST set <b>Open.Stream.IsEncrypted</b> to TRUE.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.Attributes</b>.FILE_ATTRIBUTE_ENCRYPTED is FALSE:</p>

<ul><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED
to TRUE.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.PendingNotifications</b>.FILE_NOTIFY_CHANGE_ATTRIBUTES
to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>Else: // <b>InputBuffer.EncryptionOperation</b> ==
STREAM_CLEAR_ENCRYPTION</p>

<ul><li><p><span><span>  </span></span>If <b>Open.Stream.IsEncrypted</b>
is TRUE:</p>

<ul><li><p><span><span> 
</span></span>The object store MUST set <b>Open.Stream.IsEncrypted</b> to
FALSE.</p>

</li><li><p><span><span> 
</span></span>If there does not exist an <i>ExistingStream</i> in <b>Open.File.StreamList</b>
such that <i>ExistingStream</i>.<b>IsEncrypted</b> is TRUE:</p>

<ul><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_ENCRYPTED
to FALSE.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.PendingNotifications</b>.FILE_NOTIFY_CHANGE_ATTRIBUTES
to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>The object store MUST update the duplicated information as
specified in section <a href="7e375703-5641-48f3-b844-c2ef1ee70461.html">2.1.4.18</a>
with <b>Link</b> equal to <b>Open.Link</b>.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.PendingNotifications</b> is nonzero:</p>

<ul><li><p><span><span>  </span></span>Set
<i>FilterMatch</i> = (<b>Open.File.PendingNotifications</b> | <b>Open.Link.PendingNotifications</b>).</p>

</li><li><p><span><span>  </span></span>Send
directory change notification as specified in section <a href="7f757efa-ba81-4c0e-a4c7-d11d7beed109.html">2.1.4.1</a>, with <b>Volume</b>
equal to <b>Open.File.Volume</b>, <b>Action</b> equal to FILE_ACTION_MODIFIED, <b>FilterMatch</b>
equal to <i>FilterMatch</i>, and <b>FileName</b> equal to <b>Open.FileName</b>.</p>

</li><li><p><span><span>  </span></span>For
each <i>ExistingLink</i> in <b>Open.Link.ParentFile.DirectoryList</b>:</p>

<ul><li><p><span><span> 
</span></span>If <i>ExistingLink</i> is not equal to <b>Open.Link</b>:</p>

<ul><li><p><span><span> 
</span></span><i>ExistingLink</i>.<b>PendingNotifications</b> |= <b>Open.File.PendingNotifications</b></p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul></li><li><p><span><span>  </span></span>EndFor</p>

</li><li><p><span><span>  </span></span>Set
<b>Open.Link.PendingNotifications</b> to zero.</p>

</li><li><p><span><span>  </span></span>Set
<b>Open.File.PendingNotifications</b> to zero.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If the <b>Oplock</b> member of the <b>DirectoryStream</b> in <b>Open.Link.ParentFile.StreamList</b>
(hereinafter referred to as <i>ParentOplock</i>) is not empty, the object store
MUST check for an oplock break on the parent according to the algorithm in
section <a href="306239fb-cb60-49fe-b293-df4d1a5f757a.html">2.1.4.12</a>, with
input values as follows:</p>

<ul><li><p><span><span>  </span></span><b>Open</b>
equal to this operation's <b>Open</b></p>

</li><li><p><span><span>  </span></span><b>Oplock</b>
equal to <i>ParentOplock</i></p>

</li><li><p><span><span>  </span></span><b>Operation</b>
equal to &quot;FS_CONTROL&quot;</p>

</li><li><p><span><span>  </span></span><b>OpParams</b>
containing a member <b>ControlCode</b> containing
&quot;FSCTL_SET_ENCRYPTION&quot;</p>

</li><li><p><span><span>  </span></span><b>Flags</b>
equal to &quot;PARENT_OBJECT&quot;</p>

</li></ul></li><li><p><span><span> 
</span></span>The object store MUST post a USN change as specified in section <a href="2c897c5e-b29e-464d-825f-565ff587f7f1.html">2.1.4.11</a> with <b>File</b>
equal to <b>File</b>, <b>Reason</b> equal to USN_REASON_ENCRYPTION_CHANGE, and <b>FileName</b>
equal to <b>Open.Link.Name</b>.</p>

</li><li><p><span><span> 
</span></span>If <i>ChangedFileEncryption</i> is TRUE:</p>

<ul><li><p><span><span>  </span></span>If <b>Open.UserSetChangeTime</b>
is FALSE, update <b>Open.File.LastChangeTime</b> to the current time.</p>

</li><li><p><span><span>  </span></span>Set
<b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_ARCHIVE to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Upon successful completion of this operation, the object store
MUST return:</p>

<ul><li><p><span><span>  </span></span><b>Status</b>
set to STATUS_SUCCESS.</p>

</li></ul></li></ul>
                </div>
            </div>
        </div>
    </body>
</html>