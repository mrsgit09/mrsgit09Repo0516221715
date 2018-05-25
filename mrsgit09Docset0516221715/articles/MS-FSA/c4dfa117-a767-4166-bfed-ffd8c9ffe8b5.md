<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.9.26 FSCTL_SET_DEFECT_MANAGEMENT</title>
        <xml>
            <mshelp:toctitle title="2.1.5.9.26 FSCTL_SET_DEFECT_MANAGEMENT"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: FSCTL_SET_DEFECT_MANAGEMENT"></mshelp:rltitle>
            <mshelp:keyword index="A" term="c4dfa117-a767-4166-bfed-ffd8c9ffe8b5"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="c4dfa117-a767-4166-bfed-ffd8c9ffe8b5"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: FSCTL_SET_DEFECT_MANAGEMENT" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.9.26 FSCTL_SET_DEFECT_MANAGEMENT</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The server provides:</p>

<ul><li><p><span><span> 
</span></span><b>Open:</b> An <b>Open</b> of a DataStream.</p>

</li><li><p><span><span> 
</span></span><b>InputBuffer:</b> An array of bytes containing a Boolean as
specified in <mshelp:link keywords="efbfe127-73ad-4140-9967-ec6500e66d5e" tabindex="0">[MS-FSCC]</mshelp:link>
section <mshelp:link keywords="bf78ff7e-b0a4-4ba9-8825-4af43682eb0d" tabindex="0">2.3.55</mshelp:link>.</p>

</li><li><p><span><span> 
</span></span><b>InputBufferSize:</b> The number of bytes in <b>InputBuffer</b>.</p>

</li></ul><p>On completion, the object store MUST return:</p>

<ul><li><p><span><span> 
</span></span><b>Status:</b> An NTSTATUS code that specifies the result.</p>

</li></ul><p>Support for this operation is optional. If the object store
does not implement this functionality or the target media is not a software
defect-managed media, the operation MUST be failed with
STATUS_INVALID_DEVICE_REQUEST.<a id="Appendix_A_Target_100"></a><a href="4e3695bd-7574-4f24-a223-b4679c065b63.html#Appendix_A_100" aria-label="Product behavior note 100">&lt;100&gt;</a></p>

<p>Pseudocode for the operation is as follows:</p>

<ul><li><p><span><span> 
</span></span>If <b>Open.Stream.StreamType</b> is DirectoryStream, the
operation MUST be failed with STATUS_INVALID_PARAMETER.</p>

</li><li><p><span><span> 
</span></span>If <b>InputBufferSize</b> is less than <b><i>sizeof(</i></b>Boolean<b><i>)</i></b>
(1 byte), the operation MUST be failed with STATUS_INVALID_PARAMETER.</p>

</li><li><p><span><span> 
</span></span>If <b>Open.File.OpenList</b> contains more than one Open on this
stream, this operation MUST be failed with STATUS_SHARING_VIOLATION.</p>

</li><li><p><span><span> 
</span></span>The object store MUST set <b>Open.File.DisableDefectManagement</b>
to <b>InputBuffer.Disable</b>.</p>

</li><li><p><span><span> 
</span></span>Upon successful completion of the operation, the object store
MUST return:</p>

<ul><li><p><span><span>  </span></span><b>Status</b>
set to STATUS_SUCCESS.</p>

</li></ul></li></ul>
                </div>
            </div>
        </div>
    </body>
</html>