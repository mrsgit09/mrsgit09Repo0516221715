<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.193 NumericIndicatorRange</title>
        <xml>
            <mshelp:toctitle title="2.193 NumericIndicatorRange"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: NumericIndicatorRange"></mshelp:rltitle>
            <mshelp:keyword index="A" term="3ebf4cc8-aa9f-4dfe-a97d-df0d02d74e36"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="3ebf4cc8-aa9f-4dfe-a97d-df0d02d74e36"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: NumericIndicatorRange" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.193 NumericIndicatorRange</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>NumericIndicatorRange</b> element is ignored.</p>

<p>The following are the parent elements, attributes, and child
elements of the <b>NumericIndicatorRange</b> element.</p>

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
  <p> <a href="59efa9a2-aafc-4c54-9ab2-65613de712ed.html">NumericIndicatorRanges</a>
  </p>
  </td>
 </tr>
</table>

<p> </p>

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
  <p><a href="0700b85e-3022-4332-ac90-f2f9a56aea3f.html">NumericIndicatorRange.Name</a></p>
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
  <p> <a href="ba8aba3b-4363-4990-bce1-180487628a5c.html">NumericIndicatorRange.StartValue</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p> <a href="d516a144-fab6-4f0f-8a4a-b65af5c707a7.html">NumericIndicatorRange.EndValue</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p> <a href="a48c5151-99ed-43e7-85b6-7d9553095f68.html">NumericIndicatorRange.DecimalDigitColor</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p> <a href="5c83c8e7-0466-4c49-bb00-6479672183ee.html">NumericIndicatorRange.DigitColor</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>NumericIndicatorRange</b>
element in RDL 2008/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;NumericIndicatorRangeType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;StartValue&quot; type=&quot;GaugeInputValueType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;EndValue&quot; type=&quot;GaugeInputValueType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DecimalDigitColor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DigitColor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:attribute name=&quot;Name&quot; type=&quot;xsd:normalizedString&quot; use=&quot;required&quot; /&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>NumericIndicatorRange</b>
element in RDL 2010/01 and RDL 2016/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;NumericIndicatorRangeType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;StartValue&quot; type=&quot;GaugeInputValueType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;EndValue&quot; type=&quot;GaugeInputValueType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DecimalDigitColor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DigitColor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:attribute name=&quot;Name&quot; type=&quot;xsd:normalizedString&quot; use=&quot;required&quot; /&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>