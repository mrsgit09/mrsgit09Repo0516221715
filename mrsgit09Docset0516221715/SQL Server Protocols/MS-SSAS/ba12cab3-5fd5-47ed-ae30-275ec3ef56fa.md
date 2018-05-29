<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.1.1.1.3 xmla-ds:CellInfo Complex Type</title>
        <xml>
            <mshelp:toctitle title="2.2.4.1.1.1.3 xmla-ds:CellInfo Complex Type"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: xmla-ds:CellInfo Complex Type"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ba12cab3-5fd5-47ed-ae30-275ec3ef56fa"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ba12cab3-5fd5-47ed-ae30-275ec3ef56fa"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: xmla-ds:CellInfo Complex Type" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.1.1.1.3 xmla-ds:CellInfo Complex Type</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>CellInfo</b> complex type describes the properties of
a data cell that will appear in the <b>CellData</b> section of a specific <b>mddataset</b>
return result.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;CellInfo&quot;&gt;
       &lt;xsd:sequence&gt;
         &lt;xsd:any namespace=&quot;##targetNamespace&quot; minOccurs=&quot;0&quot;
                  maxOccurs=&quot;unbounded&quot; processContents=&quot;skip&quot; /&gt;
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
  <p>xsd:any</p>
  </td>
  <td>
  <p>This complex type is a variable number of elements of
  type <b>xsd:any</b>. There will be one element for each property that is
  returned in the <b>CellData</b> section of this <b>mddataset</b> result. The
  number of elements present depends upon the number of properties that were
  requested in the query that was executed.</p>
  </td>
 </tr>
</table>

<p>The elements returned also have the following XML
attributes, with the following interpretations.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Attribute</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>Name</p>
  </td>
  <td>
  <p>The <b>Name</b> of the property on the server. This
  name cannot be the same as the element name.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Type</p>
  </td>
  <td>
  <p>The type that the element in the <b>CellData</b>
  section of the <b>mddataset</b> result will have.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>