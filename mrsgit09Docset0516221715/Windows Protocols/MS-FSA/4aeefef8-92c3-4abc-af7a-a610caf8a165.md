<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.9.31 FSCTL_SET_REPARSE_POINT</title>
        <xml>
            <mshelp:toctitle title="2.1.5.9.31 FSCTL_SET_REPARSE_POINT"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: FSCTL_SET_REPARSE_POINT"></mshelp:rltitle>
            <mshelp:keyword index="A" term="4aeefef8-92c3-4abc-af7a-a610caf8a165"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="4aeefef8-92c3-4abc-af7a-a610caf8a165"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: FSCTL_SET_REPARSE_POINT" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.9.31 FSCTL_SET_REPARSE_POINT</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The server provides:</p>

<ul><li><p><span><span> 
</span></span><b>Open:</b> An <b>Open</b> of a DataFile or DirectoryFile.</p>

</li><li><p><span><span> 
</span></span><b>InputBufferSize:</b> The byte count of the <b>InputBuffer</b>.</p>

</li><li><p><span><span> 
</span></span><b>InputBuffer:</b> An array of bytes containing a
REPARSE_DATA_BUFFER or REPARSE_GUID_DATA_BUFFER structure as defined in <mshelp:link keywords="efbfe127-73ad-4140-9967-ec6500e66d5e" tabindex="0">[MS-FSCC]</mshelp:link>
sections <mshelp:link keywords="c3a420cb-8a72-4adf-87e8-eee95379d78f" tabindex="0">2.1.2.2</mshelp:link>
and <mshelp:link keywords="a4d08374-0e92-43e2-8f88-88b94112f070" tabindex="0">2.1.2.3</mshelp:link>,
respectively.</p>

</li></ul><p>On completion, the object store <b>MUST</b> return:</p>

<ul><li><p><span><span> 
</span></span><b>Status:</b> An NTSTATUS code that specifies the result.</p>

</li></ul><p>Support for this operation is optional. If the object store
does not implement this functionality, the operation MUST be failed with
STATUS_INVALID_DEVICE_REQUEST.<a id="Appendix_A_Target_109"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.html#Appendix_A_109" aria-label="Product behavior note 109">&lt;109&gt;</a></p>

<p>Pseudocode for the operation is as follows:</p>

<ul><li><p><span><span> 
</span></span>Phase 1 -- Verify the parameters</p>

</li><li><p><span><span> 
</span></span>If (<b>Open.GrantedAccess</b> &amp; (FILE_WRITE_DATA |
FILE_WRITE_ATTRIBUTES)) == 0, the operation MUST be failed with
STATUS_ACCESS_DENIED.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.Volume.IsReadOnly</b> is TRUE, the operation MUST
be failed with STATUS_MEDIA_WRITE_PROTECTED.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.Volume.IsReparsePointsSupported</b> is FALSE, the
operation MUST be failed with STATUS_VOLUME_NOT_UPGRADED.</p>

</li><li><p><span><span> 
</span></span>If <b>InputBufferSize</b> is smaller than 8 bytes, the operation
MUST be failed with STATUS_IO_REPARSE_DATA_INVALID.</p>

</li><li><p><span><span> 
</span></span>If <b>InputBufferSize</b> is larger than 16384 bytes, the
operation MUST be failed with STATUS_IO_REPARSE_DATA_INVALID.</p>

</li><li><p><span><span> 
</span></span>If (<b>InputBufferSize</b> != <b>InputBuffer.ReparseDataLength</b>
+ 8) &amp;&amp; (<b>InputBufferSize</b> != <b>InputBuffer.ReparseDataLength</b>
+ 24), the operation MUST be failed with STATUS_IO_REPARSE_DATA_INVALID.</p>

</li><li><p><span><span> 
</span></span>If <b>InputBuffer.ReparseTag</b> == IO_REPARSE_TAG_MOUNT_POINT
and <b>Open.File.FileType</b> != DirectoryFile, the operation MUST be failed
with STATUS_NOT_A_DIRECTORY.</p>

</li><li><p><span><span> 
</span></span>If <b>InputBuffer.ReparseTag</b> == IO_REPARSE_TAG_SYMLINK and <b>Open.HasCreateSymbolicLinkAccess</b>
is FALSE, the operation MUST be failed with STATUS_ACCESS_DENIED.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.FileType</b> == DirectoryFile and <b>Open.File.DirectoryList</b>
is not empty, the operation MUST be failed with STATUS_DIRECTORY_NOT_EMPTY.</p>

</li><li><p><span><span> 
</span></span><b>If Open.File.FileType</b> == DataFile and <b>InputBuffer.ReparseTag</b>
== IO_REPARSE_TAG_SYMLINK and <b>Open.Stream.Size</b> is nonzero, the operation
MUST be failed with STATUS_IO_REPARSE_DATA_INVALID.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.FileAttributes.</b>FILE_ATTRIBUTE_REPARSE_POINT
is not set and <b>Open.File.ExtendedAttributesLength</b> is nonzero, the
operation MUST be failed with STATUS_EAS_NOT_SUPPORTED.</p>

</li><li><p><span><span> 
</span></span>Phase 2 -- Update the File</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.ReparseTag</b> is not empty (indicating that a <a href="682f0f59-385c-4351-b81a-3b234f53db03.html#gt_4fed0b53-5fc8-4818-886f-93d87f3035e1">reparse point</a> is already
assigned):</p>

<ul><li><p><span><span>  </span></span>If <b>Open.File.ReparseTag</b>
!= <b>InputBuffer.ReparseTag</b>, the operation MUST be failed with
STATUS_IO_REPARSE_TAG_MISMATCH.</p>

</li><li><p><span><span>  </span></span>If <b>Open.File.ReparseTag</b>
is a non-Microsoft tag and <b>Open.File.ReparseGUID</b> is not equal to <b>InputBuffer.ReparseGUID</b>,
the operation MUST be failed with STATUS_REPARSE_ATTRIBUTE_CONFLICT.</p>

</li><li><p><span><span>  </span></span>Copy
<b>InputBuffer.DataBuffer</b> to <b>Open.File.ReparseData</b>.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else</p>

<ul><li><p><span><span>  </span></span>Set
<b>Open.File.ReparseTag</b> to <b>InputBuffer.ReparseTag</b>.</p>

</li><li><p><span><span>  </span></span>If <b>InputBuffer.ReparseTag</b>
is a non-Microsoft Tag, then set <b>Open.File.ReparseGUID</b> to <b>InputBuffer.ReparseGUID</b>.</p>

</li><li><p><span><span>  </span></span>Set
<b>Open.File.ReparseData</b> to <b>InputBuffer.ReparseData</b>.</p>

</li><li><p><span><span>  </span></span>Set
<b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_REPARSE_POINT to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.FileType</b> == DataFile, set <b>Open.File.FileAttributes</b>.FILE_ATTRIBUTE_ARCHIVE
to TRUE.</p>

</li><li><p><span><span> 
</span></span>Update <b>Open.File.LastChangeTime</b> to the current system
time.<a id="Appendix_A_Target_110"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.html#Appendix_A_110" aria-label="Product behavior note 110">&lt;110&gt;</a></p>

</li></ul><p>Upon successful completion of the operation, the object
store MUST return:</p>

<ul><li><p><span><span> 
</span></span><b>Status</b> set to STATUS_SUCCESS.</p>

</li></ul>
                </div>
            </div>
        </div>
    </body>
</html>