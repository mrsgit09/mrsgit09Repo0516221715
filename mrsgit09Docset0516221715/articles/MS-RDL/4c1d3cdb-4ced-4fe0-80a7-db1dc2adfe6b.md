<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.129.1 ChartBorderSkin.ChartBorderSkinType</title>
        <xml>
            <mshelp:toctitle title="2.129.1 ChartBorderSkin.ChartBorderSkinType"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: ChartBorderSkin.ChartBorderSkinType"></mshelp:rltitle>
            <mshelp:keyword index="A" term="4c1d3cdb-4ced-4fe0-80a7-db1dc2adfe6b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="4c1d3cdb-4ced-4fe0-80a7-db1dc2adfe6b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: ChartBorderSkin.ChartBorderSkinType" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.129.1 ChartBorderSkin.ChartBorderSkinType</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>ChartBorderSkin.ChartBorderSkinType</b> element
specifies the <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_38e5e1a0-1189-42d7-a373-9f03a2cee49d">border skin</a>
type for a <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.html">Chart</a>. This
element is optional. If the <b>ChartBorderSkin.ChartBorderSkinType</b> element
is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) or an expression that evaluates to a <b>String</b>. The value of this
element MUST be one of the following or an expression that evaluates to one of
the following:</p>

<p><b>None</b>: Specifies no border skin.</p>

<p><b>Emboss</b>: Specifies an embossed border skin.</p>

<p><b>Raised</b>: Specifies a raised border skin.</p>

<p><b>Sunken</b>: Specifies a sunken border skin.</p>

<p><b>FrameThin1</b>: Specifies the FrameThin1 border
skin.</p>

<p><b>FrameThin2</b>: Specifies the FrameThin2 border
skin.</p>

<p><b>FrameThin3</b>: Specifies the FrameThin3 border
skin.</p>

<p><b>FrameThin4</b>: Specifies the FrameThin4 border
skin.</p>

<p><b>FrameThin5</b>: Specifies the FrameThin5 border
skin.</p>

<p><b>FrameThin6</b>: Specifies the FrameThin6 border
skin.</p>

<p><b>FrameTitle1</b>: Specifies the FrameTitle1 border
skin.</p>

<p><b>FrameTitle2</b>: Specifies the FrameTitle2 border
skin.</p>

<p><b>FrameTitle3</b>: Specifies the FrameTitle3 border
skin.</p>

<p><b>FrameTitle4</b>: Specifies the FrameTitle4 border
skin.</p>

<p><b>FrameTitle5</b>: Specifies the FrameTitle5 border
skin.</p>

<p><b>FrameTitle6</b>: Specifies the FrameTitle6 border
skin.</p>

<p><b>FrameTitle7</b>: Specifies the FrameTitle7 border
skin.</p>

<p><b>FrameTitle8</b>: Specifies the FrameTitle8 border
skin.</p>

<p>If the <b>ChartBorderSkin.ChartBorderSkinType</b> element is
not present, its value is interpreted as &quot;None&quot;.</p>

<p>The following is the parent element of the <b>ChartBorderSkin.ChartBorderSkinType</b>
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
  <p><a href="837ccfbc-ec49-4b27-97e6-0cf28f8ef1a6.html">ChartBorderSkin</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>ChartBorderSkin.ChartBorderSkinType</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;ChartBorderSkinType&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>