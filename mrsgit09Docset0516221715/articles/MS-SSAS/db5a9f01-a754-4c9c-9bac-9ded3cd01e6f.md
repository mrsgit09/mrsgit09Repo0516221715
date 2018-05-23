<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.2.2.10.2 CalculationPropertiesVisualizationProperties</title>
        <xml>
            <mshelp:toctitle title="2.2.4.2.2.10.2 CalculationPropertiesVisualizationProperties"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: CalculationPropertiesVisualizationProperties"></mshelp:rltitle>
            <mshelp:keyword index="A" term="db5a9f01-a754-4c9c-9bac-9ded3cd01e6f"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="db5a9f01-a754-4c9c-9bac-9ded3cd01e6f"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: CalculationPropertiesVisualizationProperties" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.2.2.10.2 CalculationPropertiesVisualizationProperties</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>CalculationPropertiesVisualizationProperties</b>
complex type specifies visualization properties for a calculated result. This
type is defined in the <b>eng300</b> namespace.</p>

<p>The following is the XSD for the <b>CalculationPropertiesVisualizationProperties</b>
complex type. </p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;CalculationPropertiesVisualizationProperties&quot;&gt;
     &lt;xsd:sequence&gt;
       &lt;xsd:element name=&quot;FolderPosition&quot; type=&quot;xsd:integer&quot; 
                    minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;-1&quot;/&gt;
       &lt;xsd:element name=&quot;ContextualNameRule&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;None&quot;&gt;
         &lt;xsd:simpleType&gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
             &lt;xsd:enumeration value=&quot;None&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Context&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Merge&quot; /&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;Alignment&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;Default&quot;&gt;
         &lt;xsd:simpleType&gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
             &lt;xsd:enumeration value=&quot;Default&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Left&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Right&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Center&quot; /&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;IsFolderDefault&quot; type=&quot;xsd:boolean&quot; 
                    minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;false&quot;/&gt;
       &lt;xsd:element name=&quot;IsRightToLeft&quot; type=&quot;xsd:boolean&quot; 
                    minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;false&quot;/&gt;
       &lt;xsd:element name=&quot;SortDirection&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;Default&quot;&gt;
         &lt;xsd:simpleType &gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
             &lt;xsd:enumeration value=&quot;Default&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Ascending&quot; /&gt;
             &lt;xsd:enumeration value=&quot;Descending&quot; /&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:element name=&quot;Units&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;&quot;/&gt;
       &lt;xsd:element name=&quot;Width&quot; type=&quot;xsd:integer&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;-1&quot;/&gt;
       &lt;xsd:element name=&quot;IsDefaultMeasure&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; 
                    maxOccurs=&quot;1&quot; default=&quot;false&quot;/&gt;
       &lt;xsd:element name=&quot;DefaultDetailsPosition&quot; type=&quot;xsd:integer&quot; 
                    minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;-1&quot;/&gt;
       &lt;xsd:element name=&quot;SortPropertiesPosition&quot; type=&quot;xsd:integer&quot; 
                    minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;-1&quot;/&gt;
       &lt;xsd:element name=&quot;IsSimpleMeasure&quot; type=&quot;xsd:boolean&quot; 
                    minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; default=&quot;false&quot; /&gt;
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
   <p>Read-only</p>
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
  <p>FolderPosition</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>-1</p>
  </td>
  <td>
  <p>Provides a hint to client applications to suggest the
  position that this attribute might hold among the other elements that share
  the same display folder (<a href="bc64ec5e-f9c8-4666-9d31-fdb755d87ad2.htm">AttributeTranslation</a>).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ContextualNameRule</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>&quot;None&quot;</p>
  </td>
  <td>
  <p>Provides a hint to client applications to suggest how
  to create unambiguous names for this attribute. The following values are
  allowed:</p>
  <ul><li><p><span><span>  
  </span></span><span>&quot;None&quot; – Use the
  attribute name</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Context&quot; – Use the
  incoming relationship name.</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Merge&quot; – Attending to
  language grammar, concatenate the incoming relationship name and the
  attribute name.</span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>Alignment</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>&quot;Default&quot;</p>
  </td>
  <td>
  <p>Provides a hint to client applications to suggest how
  to justify this attribute when displayed. The following values are allowed:</p>
  <ul><li><p><span><span>  
  </span></span><span>&quot;Default&quot; – Use the
  alignment appropriate for the attribute’s data type.</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Left&quot; – Align left.</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Right&quot; – Align right.</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Center&quot; – Center.</span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>IsFolderDefault</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>False</p>
  </td>
  <td>
  <p>Provides a hint to client applications that this
  attribute is representative of its display folder.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IsRightToLeft</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>False</p>
  </td>
  <td>
  <p>Provides a hint to client applications that this
  attribute is to be displayed right-to-left. </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>SortDirection</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>&quot;Default&quot;</p>
  </td>
  <td>
  <p>Provides a hint to client applications to suggest how
  to sort instances of this attribute. The following values are allowed:</p>
  <ul><li><p><span><span>  
  </span></span><span>&quot;Default&quot; – Use the
  sort direction appropriate for the attribute’s data type.</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Ascending&quot; – Sort in
  ascending order.</span></p>
  </li><li><p><span><span>  
  </span></span><span>&quot;Descending&quot; – Sort in
  descending order.</span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>Units</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Empty</p>
  </td>
  <td>
  <p>Provides a hint to client applications to suggest a string
  to be associated with values of this attribute</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Width</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>-1</p>
  </td>
  <td>
  <p>Provides a hint to client applications to suggest the
  length (in characters) to reserve to display this attribute.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IsDefaultMeasure</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Provides a hint to client applications that this <b>CalculationProperty</b>
  contains a result that is uniquely representative of a <b>Dimension</b>
  instance that the <b>CalculationProperty</b> is associated with.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DefaultDetailsPosition</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>-1</p>
  </td>
  <td>
  <p>Provides the ability to place this attribute in the
  Default Details collection of the <a href="ed122253-df54-42a8-8905-0faa6e696b8b.htm">Dimension</a>. This
  collection is an ordered set of <a href="2865fe4f-5fbb-4ae6-b0cf-811b32b4a139.htm">DimensionAttribute</a>
  types, <b>CalculationProperty</b> types, and <b>RelationshipEnd</b> elements.
  A positive value specifies participation in the collection. The collection is
  sorted in ascending order of this element.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>SortPropertiesPosition</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Provides the ability to place this attribute in the
  Sort Properties collection of the <b>Dimension</b>. This collection is an
  ordered set of <b>DimensionAttribute</b> types, <b>CalculationProperty</b>
  types, and <b>RelationshipEnd</b> elements. </p>
  <p>Client applications can interpret this collection as a
  suggestion for how to perform a multi-column sort on this <b>Dimension</b>. A
  positive value specifies participation in the collection. The collection is
  sorted in ascending order of this element.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IsSimpleMeasure</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Provides a hint to client applications that this <b>CalculationProperty</b>
  need not be displayed in clients. For example, a client might mark an automatically
  generated calculation as IsSimple so that it remains visible to the client,
  but is filtered out of any user views.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>