<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.58 MatrixColumn</title>
        <xml>
            <mshelp:toctitle title="2.58 MatrixColumn"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MatrixColumn"></mshelp:rltitle>
            <mshelp:keyword index="A" term="6fac9dfd-e5b6-4cf9-bb09-48b375eeccb8"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="6fac9dfd-e5b6-4cf9-bb09-48b375eeccb8"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MatrixColumn" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.58 MatrixColumn</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.html"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.html"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>MatrixColumn</b> element specifies a column in the
detail section of a <a href="25419c0a-c7c6-43d7-8ca5-1af842666dcb.html">Matrix</a>.</p>

<p>The following are the parent and child elements of the <b>MatrixColumn</b>
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
  <p><a href="f7861a0c-2518-4980-aa18-15abb3116c8c.html">MatrixColumns</a></p>
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
  <p><a href="ae12ba24-9134-49b0-9f44-a1c0476a4894.html">MatrixColumn.Width</a>
  </p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MatrixColumn</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;MatrixColumnType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;Width&quot; type=&quot;SizeType&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>