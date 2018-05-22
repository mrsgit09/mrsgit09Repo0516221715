<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.51.2 ColumnGrouping.FixedHeader</title>
        <xml>
            <mshelp:toctitle title="2.51.2 ColumnGrouping.FixedHeader"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: ColumnGrouping.FixedHeader"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8de6cbd3-6c4e-440d-b0ab-db161b86fc8f"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8de6cbd3-6c4e-440d-b0ab-db161b86fc8f"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: ColumnGrouping.FixedHeader" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.51.2 ColumnGrouping.FixedHeader</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.htm"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>ColumnGrouping.FixedHeader</b> element specifies
whether the header for a column grouping remains visible when a <a href="25419c0a-c7c6-43d7-8ca5-1af842666dcb.htm">Matrix</a> is partially
scrolled off the <a href="b5e525d5-00d6-4e1a-8813-55f327da6b4c.htm">Page</a>.
Fixed headers MUST be contiguous and MUST include the outermost grouping.</p>

<p>This element is optional. The value of this element MUST be
a <a href="4802fa14-3619-43fa-9898-3acab160a24c.htm">Boolean</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.2). If this element is not present, its value is interpreted as false.</p>

<p>Following is the parent element of the <b>ColumnGrouping.FixedHeader</b>
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
  <p><a href="dc090e7a-cb5f-477c-9157-b1a087d66cfc.htm">ColumnGrouping</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>ColumnGrouping.FixedHeader</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;FixedHeader&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>