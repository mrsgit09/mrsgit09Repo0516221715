<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.70 TableRows</title>
        <xml>
            <mshelp:toctitle title="2.70 TableRows"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: TableRows"></mshelp:rltitle>
            <mshelp:keyword index="A" term="e0f8c5a6-4cdb-4fec-9bfc-cabf5ecd04ad"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="e0f8c5a6-4cdb-4fec-9bfc-cabf5ecd04ad"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: TableRows" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.70 TableRows</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.htm"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.htm"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>TableRows</b> element specifies a collection of <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.htm#gt_d3a7da8d-a597-4838-9756-25e30b640ba7">table</a> rows as an ordered
list. If the <b>TableRows</b> element is specified, there MUST be at least one
and there can be more than one <a href="839c6688-01b5-4468-a398-49a7a4ce5eed.htm">TableRow</a> in the <b>TableRows</b>
collection.</p>

<p>The following are the parent and child elements of the <b>TableRows</b>
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
  <p><a href="10728959-73bf-46f9-b7a8-1b3612eda445.htm">Details</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="ac104947-f4a3-4119-85bb-386b6219d64b.htm">Header</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="cbfd158a-39e9-437a-9c7b-875c87155583.htm">Footer</a></p>
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
  <p><a href="7cea6e2c-4e51-413d-be6b-debfba4179e8.htm">TableRows.TableRow</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>TableRows</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;TableRowsType&quot;&gt;
   &lt;xsd:sequence&gt;
     &lt;xsd:element name=&quot;TableRow&quot; type=&quot;TableRowType&quot; maxOccurs=&quot;unbounded&quot; /&gt;
   &lt;/xsd:sequence&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>