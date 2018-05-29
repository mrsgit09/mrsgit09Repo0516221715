<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.55 StaticColumn</title>
        <xml>
            <mshelp:toctitle title="2.55 StaticColumn"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: StaticColumn"></mshelp:rltitle>
            <mshelp:keyword index="A" term="5ce81585-de46-403d-bfbf-feebaa70e46b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="5ce81585-de46-403d-bfbf-feebaa70e46b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: StaticColumn" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.55 StaticColumn</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.md"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.md"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>StaticColumn</b> element specifies a fixed column
header region in a <a href="25419c0a-c7c6-43d7-8ca5-1af842666dcb.md">Matrix</a>.</p>

<p>The following are the parent and child elements of the <b>StaticColumn</b>
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
  <p><a href="9aa555d4-c620-490b-8d47-cd3df4117cd8.md">StaticColumns</a></p>
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
  <p><a href="1076eec4-d49b-4ff8-af87-e7df17c7ca32.md">StaticColumn.ReportItems</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>StaticColumn</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;StaticColumnType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;ReportItems&quot; type=&quot;ReportItemsType&quot; /&gt;
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