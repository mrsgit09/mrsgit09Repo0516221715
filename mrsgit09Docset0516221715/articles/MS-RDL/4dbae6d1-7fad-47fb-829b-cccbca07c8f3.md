<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.241.11 MapPointLayer.MapShapefile</title>
        <xml>
            <mshelp:toctitle title="2.241.11 MapPointLayer.MapShapefile"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapPointLayer.MapShapefile"></mshelp:rltitle>
            <mshelp:keyword index="A" term="4dbae6d1-7fad-47fb-829b-cccbca07c8f3"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="4dbae6d1-7fad-47fb-829b-cccbca07c8f3"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapPointLayer.MapShapefile" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.241.11 MapPointLayer.MapShapefile</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.htm"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapPointLayer.MapShapefile</b> element specifies a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.htm#gt_acfac44c-899b-4e09-9b7b-02e9a82d4f50">shapefile</a> as the source for
the map points for the parent layer. This element is optional. This element is
ignored if the value of the <a href="c2ab976f-45a9-4d60-a228-e45942cf4246.htm">MapPointLayer.MapPoints</a>
element is specified. </p>

<p>The <b>MapPointLayer.MapShapefile</b> element cannot be
present if either of the following elements is present:</p>

<ul><li><p><span><span> 
</span></span> <a href="50f66e00-ecd7-48a7-9d10-ca15c307dba9.htm">MapPointLayer.MapSpatialDataSet</a></p>

</li><li><p><span><span> 
</span></span> <a href="e5028a82-02d1-4155-a9ab-78b7550dda05.htm">MapPointLayer.MapSpatialDataRegion</a>
</p>

</li></ul><p>The <b>MapPointLayer.MapShapefile</b> element is of type <a href="1974bea2-bd30-4ed4-8c98-06fd8ec7c9ee.htm">MapShapefile</a>.</p>

<p>Following is the parent element of the <b>MapPointLayer.MapShapefile</b>
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
  <p><a href="aa1875f4-9842-4672-86d6-306ba5a075aa.htm">MapPointLayer</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapPointLayer.MapShapefile</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;MapShapefile&quot; type=&quot;MapShapefileType&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>