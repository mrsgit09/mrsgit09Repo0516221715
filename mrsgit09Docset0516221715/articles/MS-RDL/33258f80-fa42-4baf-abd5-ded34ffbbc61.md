<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.29 TablixCell</title>
        <xml>
            <mshelp:toctitle title="2.29 TablixCell"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: TablixCell"></mshelp:rltitle>
            <mshelp:keyword index="A" term="33258f80-fa42-4baf-abd5-ded34ffbbc61"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="33258f80-fa42-4baf-abd5-ded34ffbbc61"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: TablixCell" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.29 TablixCell</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>TablixCell</b> parent element defines the content of
a cell in the <a href="3a4ea889-ce18-43be-940c-2dede59ea640.html">TablixBody</a>.</p>

<p>The following are the parent and child elements of the <b>TablixCell</b>
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
  <p><a href="68806b2c-5001-42ea-9159-3204fb6a12dc.html">TablixCells</a></p>
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
  <p><a href="a6564f5d-b478-42a7-9217-1a799e5ecd28.html">TablixCell.CellContents</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="93dad2c3-4c7f-490a-b2bd-6ac06eef05a5.html">TablixCell.DataElementName</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="54084c35-d31c-477d-b773-f3c9029e2a18.html">TablixCell.DataElementOutput</a></p>
  </td>
 </tr>
</table>

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.html"><b><i>RDL 2011/01</i></b></a></p>

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
  <p><a href="cd0d895a-ff2e-4046-b1c2-1ba5e167e0ae.html">TablixCell.DataSetName</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="94110e1c-36fa-4704-a9fc-8283e8dc8a03.html">TablixCell.Relationships</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>TablixCell</b>
element in RDL 2008/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;TablixCellType&quot;&gt;
   &lt;xsd:choice maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;CellContents&quot; type=&quot;CellContentsType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;DataElementName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;DataElementOutput&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
       &lt;xsd:simpleType&gt;
         &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
           &lt;xsd:enumeration value=&quot;Output&quot; /&gt;
           &lt;xsd:enumeration value=&quot;NoOutput&quot; /&gt;
           &lt;xsd:enumeration value=&quot;ContentsOnly&quot; /&gt;
           &lt;xsd:enumeration value=&quot;Auto&quot; /&gt;
         &lt;/xsd:restriction&gt;
       &lt;/xsd:simpleType&gt;
     &lt;/xsd:element&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>TablixCell</b>
element in RDL 2010/01and RDL 2016/01.</p>

<p><b>Note</b>:
The following XSD represents RDL macro-versioned schemas only. Possible
additions, identified earlier in this section, to base schema RDL 2010/01 from
micro-versioned schemas RDL 2011/01, RDL 2012/01, and RDL 2013/01 are provided
in sections 5.5, <a href="f165fb82-3c5a-4369-961c-128de233638c.html">5.6</a>,
and <a href="c5c219b8-4b13-4c49-9c86-6a07aab39823.html">5.7</a>, respectively.
For more information about macro- and micro-versioned schemas, see section <a href="ae14822f-9553-45f1-bacc-c0a1cbb484fb.html">2.1</a>.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;TablixCellType&quot;&gt;
   &lt;xsd:choice maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;CellContents&quot; type=&quot;CellContentsType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;DataElementName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
     &lt;xsd:element name=&quot;DataElementOutput&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
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