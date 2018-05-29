<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.254.12 MapPolygonTemplate.ScaleFactor</title>
        <xml>
            <mshelp:toctitle title="2.254.12 MapPolygonTemplate.ScaleFactor"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapPolygonTemplate.ScaleFactor"></mshelp:rltitle>
            <mshelp:keyword index="A" term="a0aabefb-eb6c-47d6-a1f1-dc189db145d8"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="a0aabefb-eb6c-47d6-a1f1-dc189db145d8"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapPolygonTemplate.ScaleFactor" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.254.12 MapPolygonTemplate.ScaleFactor</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapPolygonTemplate.ScaleFactor</b> element specifies
the scale factor for map polygons (specified by <a href="3ee27e43-26a2-4f27-9a31-d97e374d8633.md">MapPolygon</a> elements) to
which this <a href="1b048418-d7ff-4c51-b08e-30ab8d5a63c5.md">MapPolygonTemplate</a>
is applied. This element is optional. </p>

<p>If this element is present, its value MUST be a <a href="c7d0946f-992e-4abc-a304-09b53e030692.md">Float</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.4) or an expression that evaluates to a <b>Float</b>. If this element is
not present, its value is interpreted as 1.</p>

<p>Following is the parent element of the <b>MapPolygonTemplate.ScaleFactor</b>
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
  <p>MapPolygonTemplate</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapPolygonTemplate.ScaleFactor</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;ScaleFactor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>