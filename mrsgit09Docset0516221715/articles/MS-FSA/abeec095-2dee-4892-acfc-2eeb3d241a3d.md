<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.1.4.12.2 Algorithm to Compare Oplock Keys</title>
        <xml>
            <mshelp:toctitle title="2.1.4.12.2 Algorithm to Compare Oplock Keys"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-FSA]: Algorithm to Compare Oplock Keys"></mshelp:rltitle>
            <mshelp:keyword index="A" term="abeec095-2dee-4892-acfc-2eeb3d241a3d"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="abeec095-2dee-4892-acfc-2eeb3d241a3d"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-FSA]: Algorithm to Compare Oplock Keys" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.1.4.12.2 Algorithm to Compare Oplock Keys</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The inputs for this algorithm are:</p>

<ul><li><p><span><span> 
</span></span><b>OperationOpen:</b> The <b>Open</b> used in the request that
can cause an oplock to break.</p>

</li><li><p><span><span> 
</span></span><b>OplockOpen:</b> The <b>Open</b> originally used to request the
oplock, as specified in section <a href="64fd4383-f48a-488c-a28f-1ef92c64e878.html">2.1.5.17</a>.</p>

</li><li><p><span><span> 
</span></span><b>Flags:</b> If unspecified it is considered to contain 0. Valid
nonzero values are:</p>

<ul><li><p><span><span>  </span></span>PARENT_OBJECT</p>

</li></ul></li></ul><p>This algorithm returns TRUE if the appropriate oplock key
field of <b>OperationOpen</b> equals <b>OplockOpen.TargetOplockKey</b>, and
FALSE otherwise.</p>

<p>Pseudocode for the algorithm is as follows:</p>

<ul><li><p><span><span> 
</span></span>If <b>OperationOpen</b> equals <b>OplockOpen</b>:</p>

<ul><li><p><span><span>  </span></span>Return
TRUE.</p>

</li></ul></li><li><p><span><span> 
</span></span>If both <b>OperationOpen.TargetOplockKey</b> and <b>OperationOpen.ParentOplockKey</b>
are empty or both <b>OplockOpen.TargetOplockKey</b> and <b>OplockKey.ParentOplockKey</b>
are empty:</p>

<ul><li><p><span><span>  </span></span>Return
FALSE.</p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>OplockOpen.TargetOplockKey</b> is empty or</p>

<p>(<b>Flags</b> does not
contain PARENT_OBJECT and <b>OperationOpen.TargetOplockKey</b> is empty):</p>

<ul><li><p><span><span>  </span></span>Return
FALSE.</p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>Flags</b> contains PARENT_OBJECT and</p>

<p><b>OperationOpen.ParentOplockKey</b>
is empty:</p>

<ul><li><p><span><span>  </span></span>Return
FALSE.</p>

</li></ul></li><li><p><span><span> 
</span></span>If <b>Flags</b> contains PARENT_OBJECT:</p>

<ul><li><p><span><span>  </span></span>If <b>OperationOpen.ParentOplockKey</b>
equals <b>OplockOpen.TargetOplockKey</b>:</p>

<ul><li><p><span><span> 
</span></span>Return TRUE.</p>

</li></ul></li><li><p><span><span>  </span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>Return FALSE.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>Else:</p>

<ul><li><p><span><span>  </span></span>If <b>OperationOpen.TargetOplockKey</b>
equals <b>OplockOpen.TargetOplockKey</b>:</p>

<ul><li><p><span><span> 
</span></span>Return TRUE.</p>

</li></ul></li><li><p><span><span>  </span></span>Else:</p>

<ul><li><p><span><span> 
</span></span>Return FALSE.</p>

</li></ul></li><li><p><span><span>  </span></span>EndIf</p>

</li></ul></li><li><p><span><span> 
</span></span>EndIf</p>

</li></ul>
                </div>
            </div>
        </div>
    </body>
</html>