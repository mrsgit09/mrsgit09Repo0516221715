<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.5 ReportSection</title>
        <xml>
            <mshelp:toctitle title="2.5 ReportSection"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: ReportSection"></mshelp:rltitle>
            <mshelp:keyword index="A" term="96c3d25f-d8ce-4fe4-ab03-592edaa4a1da"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="96c3d25f-d8ce-4fe4-ab03-592edaa4a1da"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: ReportSection" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.5 ReportSection</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.htm"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>ReportSection</b> element specifies the structure and
layout information of a <b>ReportSection</b>. This element MUST be specified.</p>

<p>The following are the parent elements and child elements of
the <b>ReportSection</b> element.</p>

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
  <p><a href="734d5041-fe18-41a6-8701-d213086c575b.htm">ReportSections</a></p>
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
  <p><a href="cdf74c46-02ef-4ded-9ebc-e621e145b80d.htm">ReportSection.Body</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="9bbd51e2-ed21-498e-8080-88a1df1ad3b8.htm">ReportSection.Page</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="8a71282e-fac4-4158-808c-4c7995ffdefa.htm">ReportSection.Width</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="0a505a9d-0303-4969-b1b6-71b449d24eeb.htm">ReportSection.DataElementName</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="33e53a21-4dba-41eb-9e73-b670197038ac.htm">ReportSection.DataElementOutput</a></p>
  </td>
 </tr>
</table>

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.htm"><b><i>RDL 2011/01</i></b></a></p>

<table>
 <thead>
  <tr>
   <th>
   <p>Attributes</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="3fd6dfb2-203f-4158-afe6-ebbd00d39fa7.htm">ReportSection.Name</a></p>
  </td>
 </tr>
</table>

<p><b><i>Applies to </i></b><a href="f165fb82-3c5a-4369-961c-128de233638c.htm"><b><i>RDL 2012/01</i></b></a></p>

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
  <p><a href="b8269680-5fba-403b-ac99-84e8cc7705cb.htm">ReportSection.LayoutDirection</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>ReportSection</b>
element.</p>

<p><b>Note</b>: The following XSD represents RDL
macro-versioned schemas only. Possible additions, identified earlier in this
section, to base schema RDL 2010/01 from micro-versioned schemas RDL 2011/01,
RDL 2012/01, and RDL 2013/01 are provided in sections 5.5, 5.6, and <a href="c5c219b8-4b13-4c49-9c86-6a07aab39823.htm">5.7</a>, respectively. For
more information about macro- and micro-versioned schemas, see section <a href="ae14822f-9553-45f1-bacc-c0a1cbb484fb.htm">2.1</a>.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;ReportSectionType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;Body&quot; type=&quot;BodyType&quot; minOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Width&quot; type=&quot;SizeType&quot; minOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;Page&quot; type=&quot;PageType&quot; minOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;DataElementName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DataElementOutput&quot; minOccurs=&quot;0&quot;&gt;
       &lt;xsd:simpleType&gt;
         &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
           &lt;xsd:enumeration value=&quot;Output&quot; /&gt;
           &lt;xsd:enumeration value=&quot;NoOutput&quot; /&gt;
           &lt;xsd:enumeration value=&quot;ContentsOnly&quot; /&gt;
           &lt;xsd:enumeration value=&quot;Auto&quot; /&gt;
         &lt;/xsd:restriction&gt;
       &lt;/xsd:simpleType&gt;
     &lt;/xsd:element&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>