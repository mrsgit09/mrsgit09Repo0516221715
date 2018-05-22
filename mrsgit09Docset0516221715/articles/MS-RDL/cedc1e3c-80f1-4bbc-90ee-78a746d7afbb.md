<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.210.17 MapColorScale.RangeGapColor</title>
        <xml>
            <mshelp:toctitle title="2.210.17 MapColorScale.RangeGapColor"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapColorScale.RangeGapColor"></mshelp:rltitle>
            <mshelp:keyword index="A" term="cedc1e3c-80f1-4bbc-90ee-78a746d7afbb"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="cedc1e3c-80f1-4bbc-90ee-78a746d7afbb"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapColorScale.RangeGapColor" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.210.17 MapColorScale.RangeGapColor</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.htm"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapColorScale.RangeGapColor</b> element specifies the
color to be used in a <a href="fc14b477-a2d2-4048-843d-6a19beeb30bf.htm">MapColorScale</a>
to fill the undefined color divisions. This element is optional. If this
element is present, its value MUST be an <a href="b302c6a5-6023-42b1-95ed-bafcdc4b5714.htm">RdlColor</a> or an expression
that evaluates to an <b>RdlColor</b>. If this element is not present, its value
is interpreted as &quot;White&quot;.</p>

<p>The following is the parent element of the <b>MapColorScale.RangeGapColor</b>
element.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Parent elements</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>MapColorScale</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapColorScale.RangeGapColor</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;RangeGapColor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>