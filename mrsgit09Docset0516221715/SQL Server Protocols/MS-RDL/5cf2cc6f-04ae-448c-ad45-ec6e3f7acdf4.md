<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.314 Values</title>
        <xml>
            <mshelp:toctitle title="2.314 Values"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Values"></mshelp:rltitle>
            <mshelp:keyword index="A" term="5cf2cc6f-04ae-448c-ad45-ec6e3f7acdf4"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="5cf2cc6f-04ae-448c-ad45-ec6e3f7acdf4"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Values" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.314 Values</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Values</b> element specifies a set of values. For a
non-multivalue parameter (such as when <a href="c21237a1-8237-4538-a105-1f760242de1d.md">ReportParameter.MultiValue</a>
is set to &quot;false&quot;), this collection MUST contain one <b>Value</b>
element.</p>

<p>The following are the parent and child elements of the <b>Values</b>
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
  <p><a href="c3ccf500-98a5-438c-8e4f-fc5cc4b8d508.md">DefaultValue</a></p>
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
  <p><a href="6d1d760f-fc6f-4450-bacd-b0de538016fc.md">Values.Value</a>
  </p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Values</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;ValuesType&quot;&gt;
   &lt;xsd:sequence&gt;
     &lt;xsd:element name=&quot;Value&quot; type=&quot;xsd:string&quot; minOccurs=&quot;1&quot; 
                  maxOccurs=&quot;unbounded&quot; nullable=&quot;true&quot; /&gt;
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