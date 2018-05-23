<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.1.1.3 xmla-ds:CellData Complex Type</title>
        <xml>
            <mshelp:toctitle title="2.2.4.1.1.3 xmla-ds:CellData Complex Type"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: xmla-ds:CellData Complex Type"></mshelp:rltitle>
            <mshelp:keyword index="A" term="d9b958bc-c01b-4fbe-a5b9-24cacb989fb6"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="d9b958bc-c01b-4fbe-a5b9-24cacb989fb6"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: xmla-ds:CellData Complex Type" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.1.1.3 xmla-ds:CellData Complex Type</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>CellData</b> complex type contains either a
collection of <b>Cell</b> elements or a <b>CellSet</b> element. The server
typically returns a response that contains a collection of <b>Cell</b>
elements. However, when the <b>OptimizeResponse</b> flag is set to
&quot;7&quot;, the server returns <b>CellData</b> with an embedded <b>CellSet</b>.</p>

<p>The XML Schema definition (XSD) for the <b>CellData</b>
complex type is defined in the <b>CellInfo</b> element specification of the
current instance of this message.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;CellData&quot;&gt;
   &lt;xsd:sequence&gt;
      &lt;xsd:element name=&quot;Cell&quot; type=&quot;CellType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot; /&gt;
      &lt;xsd:element name=&quot;CellSet&quot; type=&quot;CellSetType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
   &lt;/xsd:sequence&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<table>
 <thead>
  <tr>
   <th>
   <p>Element</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>Cell</p>
  </td>
  <td>
  <p>Contains the output value for an individual cell in
  the result set, based on the axes that are used in the query. Each cell is
  uniquely identified by a <b>CellOrdinal</b>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>CellSet</p>
  </td>
  <td>
  <p>Contains a binary optimized result for the query.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>