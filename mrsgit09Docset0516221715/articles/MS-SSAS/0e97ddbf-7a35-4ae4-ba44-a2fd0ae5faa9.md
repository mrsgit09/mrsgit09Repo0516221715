<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.1.3.1 xmla-rs:row Complex Type</title>
        <xml>
            <mshelp:toctitle title="2.2.4.1.3.1 xmla-rs:row Complex Type"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: xmla-rs:row Complex Type"></mshelp:rltitle>
            <mshelp:keyword index="A" term="0e97ddbf-7a35-4ae4-ba44-a2fd0ae5faa9"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="0e97ddbf-7a35-4ae4-ba44-a2fd0ae5faa9"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: xmla-rs:row Complex Type" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.1.3.1 xmla-rs:row Complex Type</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>Each row element represents a row of tabular data.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;row&quot;&gt;
     &lt;xsd:sequence&gt;
       &lt;xsd:any namespace=&quot;##any&quot; minOccurs=&quot;0&quot; maxOccurs =&quot;unbounded&quot; /&gt;
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
  <p>The content of each row is variable. Each element
  within each row can be thought of as a column in a tabular return result.
  There will be one element in each row to represent one column in a tabular
  presentation. The <b>Schema</b> element within the <b>rs:root</b> element can
  be used to obtain a dictionary of elements that will appear within each row,
  and the types of the elements. Additional rows can be nested within a row
  result, to a single <a href="8676f5ce-62d4-4244-a326-634bfed4aba4.html#gt_35243297-04e4-4bb0-be03-defaf24c4246">level</a>.
  See section <a href="4b951396-fdb9-4434-a68a-83cff27cb7f4.html">2.2.4.1.3.1.1</a>
  for information on nested rows.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>