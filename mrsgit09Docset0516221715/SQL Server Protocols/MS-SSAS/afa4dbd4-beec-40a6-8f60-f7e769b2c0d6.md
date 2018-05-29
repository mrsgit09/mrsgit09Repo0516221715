<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.2.2.1.3.29.1 Columns</title>
        <xml>
            <mshelp:toctitle title="3.1.4.2.2.1.3.29.1 Columns"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: Columns"></mshelp:rltitle>
            <mshelp:keyword index="A" term="afa4dbd4-beec-40a6-8f60-f7e769b2c0d6"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="afa4dbd4-beec-40a6-8f60-f7e769b2c0d6"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: Columns" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.2.2.1.3.29.1 Columns</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>DISCOVER_PROPERTIES</b> rowset contains the following
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
  <p>PropertyName</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p>Yes</p>
  </td>
  <td>
  <p>The name of the property.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>PropertyDescription</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A description of the property.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>PropertyType</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The XSD data type of the property.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>PropertyAccessType</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The access for the property. The value can be Read,
  Write, or ReadWrite.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IsRequired</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>When true, indicates that a property is required;
  otherwise false.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Value</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The current value of the property.</p>
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
           &lt;xsd:element sql:field=&quot;PropertyName&quot; name=&quot;PropertyName&quot; type=&quot;xsd:string&quot; /&gt;
           &lt;xsd:element sql:field=&quot;PropertyDescription&quot; name=&quot;PropertyDescription&quot; 
                            type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;PropertyType&quot; name=&quot;PropertyType&quot; type=&quot;xsd:string&quot; 
                            minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;PropertyAccessType&quot; name=&quot;PropertyAccessType&quot; 
                            type=&quot;xsd:string&quot; /&gt;
           &lt;xsd:element sql:field=&quot;IsRequired&quot; name=&quot;IsRequired&quot; type=&quot;xsd:boolean&quot; 
                            minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;Value&quot; name=&quot;Value&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
         &lt;/xsd:sequence&gt;
       &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>