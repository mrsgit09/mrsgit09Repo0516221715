<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.5.5 Server Requests Querying a Directory</title>
        <xml>
            <mshelp:toctitle title="2.1.5.5 Server Requests Querying a Directory"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: Server Requests Querying a Directory"></mshelp:rltitle>
            <mshelp:keyword index="A" term="9d16fce3-0ace-41af-87ff-cd753cfb0ad3"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="9d16fce3-0ace-41af-87ff-cd753cfb0ad3"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: Server Requests Querying a Directory" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.5.5 Server Requests Querying a Directory</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The server provides:</p>

<ul><li><p><span><span> 
</span></span><b>Open:</b> An <b>Open</b> of a DirectoryStream.</p>

</li><li><p><span><span> 
</span></span><b>FileInformationClass:</b> The type of information being
queried, as specified in <mshelp:link keywords="efbfe127-73ad-4140-9967-ec6500e66d5e" tabindex="0">[MS-FSCC]</mshelp:link>
section <mshelp:link keywords="4718fc40-e539-4014-8e33-b675af74e3e1" tabindex="0">2.4</mshelp:link>.</p>

</li><li><p><span><span> 
</span></span><b>OutputBufferSize:</b> The maximum number of bytes to return in
<b>OutputBuffer</b>.</p>

</li><li><p><span><span> 
</span></span><b>RestartScan:</b> A Boolean value which, if TRUE, indicates
that enumeration is restarted from the beginning of the directory. If FALSE,
enumeration continues from the last position.</p>

</li><li><p><span><span> 
</span></span><b>ReturnSingleEntry:</b> A Boolean value which, if TRUE,
indicates that at most one entry MUST be returned. If FALSE, a variable count
of entries could be returned, not to exceed <b>OutputBufferSize</b> bytes.</p>

</li><li><p><span><span> 
</span></span><b>FileIndex:</b> An index number from which to resume the
enumeration if the object store supports it (optional).</p>

</li><li><p><span><span> 
</span></span><b>FileNamePattern:</b> A <a href="682f0f59-385c-4351-b81a-3b234f53db03.md#gt_c305d0ab-8b94-461a-bd76-13b40cb8c4d8">Unicode</a> string containing
the file name pattern to match. The object store MUST treat any asterisk
(&quot;*&quot;) and question mark (&quot;?&quot;) characters in <b>FileNamePattern</b>
as wildcards. <b>FileNamePattern</b> could be empty. The object store MUST
treat an empty value as equivalent to the pattern &quot;*&quot;.</p>

</li></ul><p>On completion, the object store MUST return:</p>

<ul><li><p><span><span> 
</span></span><b>Status:</b> An NTSTATUS code that specifies the result.</p>

</li><li><p><span><span> 
</span></span><b>OutputBuffer:</b> An array of bytes containing the query
results. The structure of these bytes is dependent on the <b>FileInformationClass</b>,
as noted in the relevant subsection.</p>

</li><li><p><span><span> 
</span></span><b>ByteCount:</b> The number of bytes stored in <b>OutputBuffer</b>.</p>

</li></ul>
                </div>
            </div>
        </div>
    </body>
</html>