<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.2.2.1.3.32.1 Columns</title>
        <xml>
            <mshelp:toctitle title="3.1.4.2.2.1.3.32.1 Columns"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: Columns"></mshelp:rltitle>
            <mshelp:keyword index="A" term="455b6dbb-2efe-4bc9-8a40-52aa38e0deec"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="455b6dbb-2efe-4bc9-8a40-52aa38e0deec"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: Columns" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.2.2.1.3.32.1 Columns</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>DISCOVER_KEYWORDS</b> rowset contains the following
columns.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Name</p>
   </th>
   <th>
   <p>Type</p>
   </th>
   <th>
   <p>Restriction</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>Keyword</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p>Yes</p>
  </td>
  <td>
  <p>The keyword string.</p>
  </td>
 </tr>
</table>

<p>This schema rowset is not sorted.</p>

<p>The response has the following definition.</p>

<dl>
<dd>
<div><pre>       &lt;xsd:element name=&quot;root&quot;&gt;
         &lt;xsd:complexType&gt;
           &lt;xsd:sequence minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
             &lt;xsd:element name=&quot;row&quot; type=&quot;row&quot; /&gt;
           &lt;/xsd:sequence&gt;
         &lt;/xsd:complexType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:complexType name=&quot;row&quot;&gt;
         &lt;xsd:sequence&gt;
           &lt;xsd:element sql:field=&quot;Keyword&quot; name=&quot;Keyword&quot; type=&quot;xsd:string&quot; /&gt;
         &lt;/xsd:sequence&gt;
       &lt;/xsd:complexType&gt;
            
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>