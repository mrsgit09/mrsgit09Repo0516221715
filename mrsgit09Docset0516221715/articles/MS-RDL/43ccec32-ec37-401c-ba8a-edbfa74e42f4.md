<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.30 CellContents</title>
        <xml>
            <mshelp:toctitle title="2.30 CellContents"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: CellContents"></mshelp:rltitle>
            <mshelp:keyword index="A" term="43ccec32-ec37-401c-ba8a-edbfa74e42f4"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="43ccec32-ec37-401c-ba8a-edbfa74e42f4"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: CellContents" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.30 CellContents</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>CellContents</b> element defines the contents of
cells of a <a href="e42fb86e-799a-4202-8845-ac38831efccb.md">Tablix</a>. The <b>CellContents</b>
element can contain 0 or 1 report item elements. If the <b>Top</b>, <b>Left</b>,
<b>Height</b>, and <b>Width</b> grandchild elements exist, they are ignored,
and their values are interpreted as follows:</p>

<p><b>Top</b>: 0</p>

<p><b>Left</b>: 0</p>

<p><b>Height</b>: The same as the height of the
containing object.</p>

<p><b>Width</b>: The same as the width of the containing
object.</p>

<p>The following are the parent and child elements of the <b>CellContents</b>
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
  <p><a href="33258f80-fa42-4baf-abd5-ded34ffbbc61.md">TablixCell</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="6cdfb648-977b-4e6a-9316-19e8d45b6c10.md">TablixCornerCell</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="ac71f119-59be-471b-9316-e95b931402cb.md">TablixHeader</a></p>
  </td>
 </tr>
</table>

<p> </p>

<table>
 <thead>
  <tr>
   <th>
   <p>Child elements</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="90926a0d-f021-4dd5-8d20-0bba6c7a1991.md">CellContents.Chart</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="3ffb0387-2dd7-4b21-b36d-6df8fd0a0887.md">CellContents.ColSpan</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="e09f0734-9dfe-48bb-8a01-83fd55737d5c.md">CellContents.CustomReportItem</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="8286c536-2fa9-4ff0-93b8-6982faa2c305.md">CellContents.GaugePanel</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="09dceeb9-3f84-499f-b37a-2f6138eed780.md">CellContents.Image</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="a6e4edf9-5630-4255-b212-276b4e5c62a6.md">CellContents.Line</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="bd1cf9f2-0bc1-46df-82b2-d23b3ca45dc1.md">CellContents.Map</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="c5a5fbb0-c109-462a-ad16-ea1600b51ae0.md">CellContents.Rectangle</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="86a03c35-d5eb-4e30-be28-f8219e73fa30.md">CellContents.RowSpan</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="8055db6b-3215-46db-b1bf-b5a4ec874e36.md">CellContents.Subreport</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="cb7cc349-acc7-4ecb-bb8c-a451d7ae1dfb.md">CellContents.Tablix</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="231b670f-37d0-4fa6-a874-cc9c52229fdd.md">CellContents.Textbox</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>CellContents</b>
element in RDL 2008/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;CellContentsType&quot;&gt;
   &lt;xsd:choice maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;ColSpan&quot; type=&quot;xsd:unsignedInt&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
     &lt;/xsd:element&gt;
     &lt;xsd:element name=&quot;RowSpan&quot; type=&quot;xsd:unsignedInt&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
     &lt;/xsd:element&gt;
     &lt;xsd:element name=&quot;Line&quot; type=&quot;LineType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Rectangle&quot; type=&quot;RectangleType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Textbox&quot; type=&quot;TextboxType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Image&quot; type=&quot;ImageType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Subreport&quot; type=&quot;SubreportType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Chart&quot; type=&quot;ChartType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;GaugePanel&quot; type=&quot;GaugePanelType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;CustomReportItem&quot; type=&quot;CustomReportItemType&quot; minOccurs=&quot;0&quot; 
                  maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Tablix&quot; type=&quot;TablixType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>CellContents</b>
element in RDL 2010/01 and RDL 2016/01.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;CellContentsType&quot;&gt;
     &lt;xsd:choice maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;ColSpan&quot; type=&quot;xsd:unsignedInt&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;RowSpan&quot; type=&quot;xsd:unsignedInt&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;Line&quot; type=&quot;LineType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Rectangle&quot; type=&quot;RectangleType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Textbox&quot; type=&quot;TextboxType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Image&quot; type=&quot;ImageType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Subreport&quot; type=&quot;SubreportType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Chart&quot; type=&quot;ChartType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;GaugePanel&quot; type=&quot;GaugePanelType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Map&quot; type=&quot;MapType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;CustomReportItem&quot; type=&quot;CustomReportItemType&quot; minOccurs=&quot;0&quot; 
                    maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:element name=&quot;Tablix&quot; type=&quot;TablixType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>