<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.12.1 FileFsVolumeInformation</title>
        <xml>
            <mshelp:toctitle title="2.1.5.12.1 FileFsVolumeInformation"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: FileFsVolumeInformation"></mshelp:rltitle>
            <mshelp:keyword index="A" term="3bbac4ba-430a-4846-b3bd-66ffdce765db"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="3bbac4ba-430a-4846-b3bd-66ffdce765db"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: FileFsVolumeInformation" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.12.1 FileFsVolumeInformation</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b>OutputBuffer</b> is of type FILE_FS_VOLUME_INFORMATION,
as described in <mshelp:link keywords="efbfe127-73ad-4140-9967-ec6500e66d5e" tabindex="0">[MS-FSCC]</mshelp:link>
section <mshelp:link keywords="bf691378-c34e-4a13-976e-404ea1a87738" tabindex="0">2.5.9</mshelp:link>.</p>

<p>This routine uses the following local variables:</p>

<ul><li><p><span><span> 
</span></span>32-bit unsigned integers: <i>RemainingLength</i>, <i>BytesToCopy</i></p>

</li></ul><p>Pseudocode for the operation is as follows:</p>

<ul><li><p><span><span> 
</span></span>If <b>OutputBufferSize</b> is smaller than <b><i>BlockAlign(FieldOffset(</i></b>FILE_FS_VOLUME_INFORMATION.VolumeLabel<b><i>)</i></b>,
8<b><i>)</i></b>, the operation MUST be failed with
STATUS_INFO_LENGTH_MISMATCH.</p>

</li><li><p><span><span> 
</span></span><b>OutputBuffer</b> MUST be constructed as follows:</p>

<ul><li><p><span><span>  </span></span><b>OutputBuffer.VolumeCreationTime</b>
set to <b>Open.File.Volume.VolumeCreationTime</b>.</p>

</li><li><p><span><span>  </span></span><b>OutputBuffer.VolumeSerialNumber</b>
set to <b>Open.File.Volume.VolumeSerialNumber</b>.</p>

</li><li><p><span><span>  </span></span><b>OutputBuffer.VolumeLabelLength</b>
set to the length, in bytes, of the <b>Open.File.Volume.VolumeLabel</b> string.
This value can be zero.</p>

</li><li><p><span><span>  </span></span><b>OutputBuffer.SupportsObjects</b>
set to TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>Set <i>RemainingLength</i> to <b>OutputBufferSize - <i>FieldOffset(</i></b>FILE_FS_VOLUME_INFORMATION.VolumeLabel<b><i>)</i></b>.</p>

</li><li><p><span><span> 
</span></span>If <i>RemainingLength</i> &lt; <b>OutputBuffer.VolumeLabelLength</b>:</p>

<ul><li><p><span><span>  </span></span>Set
<i>BytesToCopy</i> to <i>RemainingLength</i>.</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span>  </span></span>Set
<i>BytesToCopy</i> to <b>OutputBuffer.VolumeLabelLength</b>.</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li><li><p><span><span> 
</span></span>Copy <i>BytesToCopy</i> bytes from <b>Volume.VolumeLable</b> to <b>OutputBuffer.VolumeLabel</b>.</p>

</li><li><p><span><span> 
</span></span>Upon successful completion of the operation, the object store
MUST return:</p>

<ul><li><p><span><span>  </span></span><b>ByteCount</b>
set to <b><i>FieldOffset(</i></b>FILE_FS_VOLUME_INFORMATION.VolumeLabel<b><i>)</i></b>
+ <i>BytesToCopy</i>.</p>

</li><li><p><span><span>  </span></span><b>Status</b>
set to STATUS_BUFFER_OVERFLOW if <i>BytesToCopy</i> &lt; <b>OutputBuffer.VolumeLabelLength</b>
else STATUS_SUCCESS.</p>

</li></ul></li></ul>
                </div>
            </div>
        </div>
    </body>
</html>