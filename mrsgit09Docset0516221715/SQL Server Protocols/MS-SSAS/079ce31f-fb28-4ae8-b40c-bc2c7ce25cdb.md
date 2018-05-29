<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.2.2.21.1 CubeDimensionPermission</title>
        <xml>
            <mshelp:toctitle title="2.2.4.2.2.21.1 CubeDimensionPermission"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: CubeDimensionPermission"></mshelp:rltitle>
            <mshelp:keyword index="A" term="079ce31f-fb28-4ae8-b40c-bc2c7ce25cdb"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="079ce31f-fb28-4ae8-b40c-bc2c7ce25cdb"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: CubeDimensionPermission" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.2.2.21.1 CubeDimensionPermission</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>CubeDimensionPermission</b> complex type represents
permissions for a <a href="7b4ec273-230d-4558-801f-3e7dff015ddc.html">CubeDimension</a>.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;CubeDimensionPermission&quot;&gt;
     &lt;xsd:all&gt;
       &lt;xsd:element name=&quot;CubeDimensionID&quot; type=&quot;xsd:string&quot;/&gt;
       &lt;xsd:element name=&quot;Description&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;/&gt;
       &lt;xsd:element name=&quot;Read&quot; minOccurs=&quot;0&quot;&gt;
         &lt;xsd:simpleType&gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot; &gt;
             &lt;xsd:enumeration value=&quot;None&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Allowed&quot; /&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;Write&quot; minOccurs=&quot;0&quot;&gt;
         &lt;xsd:simpleType&gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot; &gt;
             &lt;xsd:enumeration value=&quot;None&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Allowed&quot; /&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;AttributePermissions&quot; minOccurs=&quot;0&quot;&gt;
         &lt;xsd:complexType&gt;
           &lt;xsd:sequence&gt;
             &lt;xsd:element name=&quot;AttributePermission&quot;  type=&quot;AttributePermission&quot;
                          minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;/&gt;
           &lt;/xsd:sequence&gt;
         &lt;/xsd:complexType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;Annotations&quot; minOccurs=&quot;0&quot;&gt;
         &lt;xsd:complexType&gt;
           &lt;xsd:sequence&gt;
             &lt;xsd:element name=&quot;Annotation&quot;  type=&quot;Annotation&quot;
                          minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;/&gt;
           &lt;/xsd:sequence&gt;
         &lt;/xsd:complexType&gt;
       &lt;/xsd:element&gt;
     &lt;/xsd:all&gt;
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
   <p>Read-Only</p>
   </th>
   <th>
   <p>Default value</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>CubeDimensionID</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>[Required]</p>
  </td>
  <td>
  <p>The ID of the <b>CubeDimension</b>. For the <b>Measures</b>
  dimension, this string MUST be set to &quot;Measures&quot;.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Description</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Empty</p>
  </td>
  <td>
  <p>The object description.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Read</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>&quot;Allowed&quot;</p>
  </td>
  <td>
  <p>Specifies whether the role has permission to read
  metadata or data from the <b>CubeDimension</b>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Write</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>&quot;None&quot;</p>
  </td>
  <td>
  <p>Specifies whether the role has permission to write to
  the <b>CubeDimension</b>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>AttributePermissions</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Empty</p>
  </td>
  <td>
  <p>A collection of <a href="c7e44b38-ff08-40a5-85ee-20944c827556.html">AttributePermission</a>
  objects.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Annotations</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Empty</p>
  </td>
  <td>
  <p>A collection of <a href="f660115e-7c55-4ee3-af55-75939f9a9b3b.html">Annotation</a> objects.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>