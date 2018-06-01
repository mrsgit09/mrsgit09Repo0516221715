<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.2.2.1.3.4.1 Columns</title>
        <xml>
            <mshelp:toctitle title="3.1.4.2.2.1.3.4.1 Columns"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: Columns"></mshelp:rltitle>
            <mshelp:keyword index="A" term="7260f6dc-bad5-4ec7-834e-5cbbc2b2fca0"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="7260f6dc-bad5-4ec7-834e-5cbbc2b2fca0"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: Columns" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.2.2.1.3.4.1 Columns</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>DBSCHEMA_PROVIDER_TYPES</b> rowset contains the
following columns.</p>

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
  <p>TYPE_NAME</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The server-specific data type name.<a id="Appendix_A_Target_179"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_179" aria-label="Product behavior note 179">&lt;179&gt;</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DATA_TYPE</p>
  </td>
  <td>
  <p>xsd:unsignedShort</p>
  </td>
  <td>
  <p>Yes</p>
  </td>
  <td>
  <p>This enumeration is the same as <b>LEVEL_DBTYPE</b>
  for <b>MDSCHEMA_LEVELS</b>. (See section <a href="bf5b4bd4-b5db-406b-b830-b3720e890b4a.md">3.1.4.2.2.1.3.8</a>)</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>COLUMN_SIZE</p>
  </td>
  <td>
  <p>xsd:unsignedInt</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The length of a non-numeric column or parameter that
  refers to either the maximum or the length defined for this type by the
  server. For character data, this is the maximum or defined length in
  characters. For <b>DateTime</b> data types, this is the length of the string
  representation (assuming the maximum allowed precision of the fractional
  second component).</p>
  <p>If the data type is numeric, this is the upper bound
  on the maximum precision of the data type.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>LITERAL_PREFIX</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The character or characters used to prefix a literal
  of this type in a text command.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>LITERAL_SUFFIX</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The character or characters used to suffix a literal
  of this type in a text command.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>CREATE_PARAMS</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The creation parameters specified by the consumer when
  creating a column of this data type. For example, the <b>SQL DECIMAL</b> data
  type needs a precision and a scale. In this case, the creation parameters
  might be the string &quot;precision,scale&quot;. In a text command to create
  a DECIMAL column with a precision of 10 and a scale of 2, the value of the
  TYPE_NAME column might be DECIMAL(), and the complete type specification
  would be DECIMAL(10,2).</p>
  <p>The creation parameters appear as a comma-separated
  list of values, in the order they are to be supplied and with no surrounding
  parentheses. If a creation parameter is length, maximum length, precision,
  scale, seed, or increment, use &quot;length&quot;, &quot;max length&quot;,
  &quot;precision&quot;, &quot;scale&quot;, &quot;seed&quot;, and
  &quot;increment&quot;, respectively. If the creation parameter is some other
  value, the server determines what text is to be used to describe the creation
  parameter.</p>
  <p>If the data type requires creation parameters,
  &quot;()&quot; usually appears in the type name. This indicates the position
  at which to insert the creation parameters. If the type name does not include
  &quot;()&quot;, the creation parameters are enclosed in parentheses and
  appended to the data type name.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IS_NULLABLE</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type is
  nullable.</p>
  <ul><li><p><span><span>  
  </span></span><span>True indicates that the data type
  is nullable.</span></p>
  </li><li><p><span><span>  
  </span></span><span>False indicates that the data
  type is not nullable.</span></p>
  </li></ul><p><span>§<span>  
  </span></span>NULL indicates that it is not known whether the data type is
  nullable.<a id="Appendix_A_Target_180"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_180" aria-label="Product behavior note 180">&lt;180&gt;</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p>CASE_SENSITIVE</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type is a
  character type and case-sensitive.</p>
  <ul><li><p><span><span>  
  </span></span><span>True indicates that the data type
  is a character type and is case-sensitive.</span></p>
  </li><li><p><span><span>  
  </span></span><span>False indicates that the data
  type is not case-sensitive.</span></p>
  </li><li><p><span><span>  
  </span></span><span>NULL indicates that the data type
  is not a character type.</span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>SEARCHABLE</p>
  </td>
  <td>
  <p>xsd:unsignedInt</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>An integer indicating how the data type can be used in
  searches if the server supports ICommandText; otherwise, NULL.</p>
  <p>If the server supports ICommandText, then this column
  can have the following values:</p>
  <ul><li><p><span><span>  
  </span></span><span>DB_UNSEARCHABLE (0x01) -
  indicates that the data type cannot be used in a WHERE clause.</span></p>
  </li><li><p><span><span>  
  </span></span><span>DB_LIKE_ONLY (0x02) - indicates
  that the data type can be used in a WHERE clause only with the LIKE
  predicate.</span></p>
  </li><li><p><span><span>  
  </span></span><span>DB_ALL_EXCEPT_LIKE (0x03) -
  indicates that the data type can be used in a WHERE clause with all
  comparison operators except LIKE.</span></p>
  </li><li><p><span><span>  
  </span></span><span>DB_SEARCHABLE (0x04) - indicates
  that the data type can be used in a WHERE clause with any comparison
  operator.<a id="Appendix_A_Target_181"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_181" aria-label="Product behavior note 181">&lt;181&gt;</a></span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>UNSIGNED_ATTRIBUTE</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type is
  unsigned.</p>
  <ul><li><p><span><span>  
  </span></span><span>True indicates that the data type
  is unsigned.</span></p>
  </li><li><p><span><span>  
  </span></span><span>False indicates that the data
  type is signed.</span></p>
  </li><li><p><span><span>  
  </span></span><span>NULL indicates that this is not
  applicable to the data type.</span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>FIXED_PREC_SCALE</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type has a
  fixed precision and scale.</p>
  <ul><li><p><span><span>  
  </span></span><span>True indicates that the data type
  has a fixed precision and scale.</span></p>
  </li><li><p><span><span>  
  </span></span><span>False indicates that the data
  type does not have a fixed precision and scale.<a id="Appendix_A_Target_182"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_182" aria-label="Product behavior note 182">&lt;182&gt;</a></span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>AUTO_UNIQUE_VALUE</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type can be
  autoincrementing.</p>
  <ul><li><p><span><span>  
  </span></span><span>True indicates that values of
  this type can be autoincrementing.</span></p>
  </li><li><p><span><span>  
  </span></span><span>False indicates that values of
  this type cannot be autoincrementing.</span></p>
  </li><li><p><span><span>  
  </span></span><span>If this value is true, the
  server's DBPROP_COL_AUTOINCREMENT column property determines whether a column
  of this type is always autoincrementing. If the DBPROP_COL_AUTOINCREMENT
  property is read/write, the setting of the DBPROP_COL_AUTOINCREMENT property
  determines whether a column of this type is autoincrementing. If
  DBPROP_COL_AUTOINCREMENT is a read-only property, either all or none of the
  columns of this type are autoincrementing.<a id="Appendix_A_Target_183"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_183" aria-label="Product behavior note 183">&lt;183&gt;</a></span></p>
  </li></ul></td>
 </tr>
 <tr>
  <td>
  <p>LOCAL_TYPE_NAME</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The localized version of TYPE_NAME. NULL is returned
  if a localized name is not supported by the server.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>MINIMUM_SCALE</p>
  </td>
  <td>
  <p>xds:short</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>If the type indicator is DBTYPE_VARNUMERIC,
  DBTYPE_DECIMAL, or DBTYPE_NUMERIC, this column specifies the minimum number
  of digits allowed to the right of the decimal point. Otherwise, it is NULL.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>MAXIMUM_SCALE</p>
  </td>
  <td>
  <p>xds:short</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>If the type indicator is DBTYPE_VARNUMERIC,
  DBTYPE_DECIMAL, or DBTYPE_NUMERIC, this column specifies the maximum number
  of digits allowed to the right of the decimal point. Otherwise, it is NULL.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>GUID</p>
  </td>
  <td>
  <p>uuid</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>(Reserved for future use.)</p>
  <p>The GUID of the type, if the type is described in a
  type library. Otherwise, it is NULL.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>TYPELIB</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The type library that contains the description of the
  type, if the type is described in a type library. Otherwise, it is NULL.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>VERSION</p>
  </td>
  <td>
  <p>xsd:string</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>The version of the type definition. Servers might
  request to create different versions of type definitions. Different servers
  might use different versioning schemes, such as a timestamp or a number (<b>Integer</b>
  or <b>Float</b>). NULL if not supported.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IS_LONG</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type is a
  binary large object (BLOB) and has very long data.</p>
  <ul><li><p><span><span>  
  </span></span><span>True indicates that the data type
  is a BLOB that contains very long data; the definition of very long data is
  server-specific.<a id="Appendix_A_Target_184"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_184" aria-label="Product behavior note 184">&lt;184&gt;</a></span></p>
  </li><li><p><span><span>  
  </span></span><span>False indicates that the data
  type is a BLOB that does not contain very long data or that is not a BLOB.</span></p>
  </li></ul><p>This column value determines the setting of the
  DBCOLUMNFLAGS_ISLONG flag that is returned by <b>GetColumnInfo</b> in <b>IColumnsInfo</b>
  and the setting of the DBCOLUMNFLAGS_ISLONG flag that is returned by <b>GetParameterInfo</b>
  in <b>ICommandWithParameters</b>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>BEST_MATCH</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p>Yes<a id="Appendix_A_Target_185"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_185" aria-label="Product behavior note 185">&lt;185&gt;</a> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the data type is the
  best match.</p>
  <p>A value of true indicates that the data type is the
  best match between all data types in the data store and the OLE DB data type
  that is indicated by the value in the DATA_TYPE column. For more information,
  see <a href="https://go.microsoft.com/fwlink/?LinkId=90054">[MSDN-OLEDB]</a>.</p>
  <p>A value of false indicates that the data type is not
  the best match.</p>
  <p>For each set of rows in which the value of the
  DATA_TYPE column is the same, the BEST_MATCH column is set to true in only
  one row.<a id="Appendix_A_Target_186"></a><a href="b9ac4859-2662-44ca-b131-9addd8b953dc.md#Appendix_A_186" aria-label="Product behavior note 186">&lt;186&gt;</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p>IS_FIXEDLENGTH</p>
  </td>
  <td>
  <p>xsd:boolean</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>A Boolean that indicates whether the column is fixed
  in length.</p>
  <p>A value of true indicates that columns of this type
  that are created by the <a href="8676f5ce-62d4-4244-a326-634bfed4aba4.md#gt_e015fbff-3760-4e33-8898-dc55fbf815d5">DDL</a>
  will be of fixed length.</p>
  <p>A value of false indicates that columns of this type
  that are created by the DDL will be of variable length.</p>
  <p>If the field is NULL, it is not known whether the
  server will map this field with a fixed-length or variable-length column.</p>
  </td>
 </tr>
</table>

<p>The rowset is not sorted.</p>

<p>The response has the following definition.</p>

<dl>
<dd>
<div><pre>      &lt;xsd:element name=&quot;root&quot;&gt;
         &lt;xsd:complexType&gt;
           &lt;xsd:sequence minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
             &lt;xsd:element name=&quot;row&quot; type=&quot;row&quot; /&gt;
           &lt;/xsd:sequence&gt;
         &lt;/xsd:complexType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:simpleType name=&quot;uuid&quot;&gt;
         &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
           &lt;xsd:pattern value=&quot;[0-9a-zA-Z]{8}-[0-9a-zA-Z]{4}-[0-9a-zA-Z]{4}-[0-9a-zA-Z]{4}-[0-9a-zA-Z]{12}&quot; /&gt;
         &lt;/xsd:restriction&gt;
       &lt;/xsd:simpleType&gt;
       &lt;xsd:complexType name=&quot;row&quot;&gt;
         &lt;xsd:sequence&gt;
           &lt;xsd:element sql:field=&quot;TYPE_NAME&quot; name=&quot;TYPE_NAME&quot; type=&quot;xsd:string&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;DATA_TYPE&quot; name=&quot;DATA_TYPE&quot; type=&quot;xsd:unsignedShort&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;COLUMN_SIZE&quot; name=&quot;COLUMN_SIZE&quot; type=&quot;xsd:unsignedInt&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;LITERAL_PREFIX&quot; name=&quot;LITERAL_PREFIX&quot; type=&quot;xsd:string&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;LITERAL_SUFFIX&quot; name=&quot;LITERAL_SUFFIX&quot; type=&quot;xsd:string&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;CREATE_PARAMS&quot; name=&quot;CREATE_PARAMS&quot; type=&quot;xsd:string&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;IS_NULLABLE&quot; name=&quot;IS_NULLABLE&quot; type=&quot;xsd:boolean&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;CASE_SENSITIVE&quot; name=&quot;CASE_SENSITIVE&quot; type=&quot;xsd:boolean&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;SEARCHABLE&quot; name=&quot;SEARCHABLE&quot; type=&quot;xsd:unsignedInt&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;UNSIGNED_ATTRIBUTE&quot; name=&quot;UNSIGNED_ATTRIBUTE&quot; 
                        type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;FIXED_PREC_SCALE&quot; name=&quot;FIXED_PREC_SCALE&quot; 
                        type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;AUTO_UNIQUE_VALUE&quot; name=&quot;AUTO_UNIQUE_VALUE&quot; 
                        type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;LOCAL_TYPE_NAME&quot; name=&quot;LOCAL_TYPE_NAME&quot; type=&quot;xsd:string&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;MINIMUM_SCALE&quot; name=&quot;MINIMUM_SCALE&quot; type=&quot;xsd:short&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;MAXIMUM_SCALE&quot; name=&quot;MAXIMUM_SCALE&quot; type=&quot;xsd:short&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;GUID&quot; name=&quot;GUID&quot; type=&quot;uuid&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;TYPELIB&quot; name=&quot;TYPELIB&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;VERSION&quot; name=&quot;VERSION&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;IS_LONG&quot; name=&quot;IS_LONG&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;BEST_MATCH&quot; name=&quot;BEST_MATCH&quot; type=&quot;xsd:boolean&quot; 
                        minOccurs=&quot;0&quot; /&gt;
           &lt;xsd:element sql:field=&quot;IS_FIXEDLENGTH&quot; name=&quot;IS_FIXEDLENGTH&quot; type=&quot;xsd:boolean&quot; 
                        minOccurs=&quot;0&quot; /&gt;
         &lt;/xsd:sequence&gt;
       &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>