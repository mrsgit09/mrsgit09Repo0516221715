<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.15 LocIDStringWithDataTypeAttribute</title>
        <xml>
            <mshelp:toctitle title="2.2.15 LocIDStringWithDataTypeAttribute"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: LocIDStringWithDataTypeAttribute"></mshelp:rltitle>
            <mshelp:keyword index="A" term="b54d0e96-1cbd-4cca-ad5f-cce0dfc355fe"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="b54d0e96-1cbd-4cca-ad5f-cce0dfc355fe"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: LocIDStringWithDataTypeAttribute" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.15 LocIDStringWithDataTypeAttribute</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>LocIDStringWithDataTypeAttribute</b> type specifies a
<a href="5164cbae-8db1-4dff-8ef1-2026f55b100a.htm">StringWithDataTypeAttribute</a>
with an <b>EvaluationMode</b> attribute. The <b>EvaluationMode</b> attribute
specifies whether the value of the <b>LocIDStringWithDataTypeAttribute</b> type
is treated as an expression or constant. The <b>EvaluationMode</b> attribute is
optional. If this attribute is present, its value MUST be one of the following:</p>

<p><b>Auto</b>: Specifies that value MUST be treated as
an expression if it starts with &quot;=&quot; and as a constant otherwise.</p>

<p><b>Constant</b>: Specifies that value MUST be treated
as a constant.</p>

<p>If the <b>EvaluationMode</b> attribute is not present, its
value is interpreted as &quot;Auto&quot;. </p>

<p>The <b>LocIDStringWithDataTypeAttribute</b> type can be
referenced by the following elements.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Referenced by</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="99982bda-2dd1-4626-b8ef-da888d95f4ff.htm">TextRun.Value</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>LocIDStringWithDataTypeAttribute</b>
type in <a href="1e855f94-4617-47e4-b89e-0856c6cb420f.htm">RDL 2008/01</a>.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;LocIDStringWithDataTypeAttribute&quot;&gt;
     &lt;xsd:simpleContent&gt;
       &lt;xsd:extension base=&quot;StringWithDataTypeAttribute&quot;&gt;
         &lt;xsd:attribute name=&quot;EvaluationMode&quot; type=&quot;EvaluationModeType&quot; default=&quot;Auto&quot; /&gt;
         &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
       &lt;/xsd:extension&gt;
     &lt;/xsd:simpleContent&gt;
   &lt;/xsd:complexType&gt;
   &lt;xsd:simpleType name=&quot;EvaluationModeType&quot;&gt;
     &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
       &lt;xsd:enumeration value=&quot;Auto&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Constant&quot; /&gt;
     &lt;/xsd:restriction&gt;
   &lt;/xsd:simpleType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>LocIDStringWithDataTypeAttribute</b>
type in <a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm">RDL 2010/01</a>
and <a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.htm">RDL 2016/01</a>.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;LocIDStringWithDataTypeAttribute&quot;&gt;
     &lt;xsd:simpleContent&gt;
       &lt;xsd:extension base=&quot;StringWithDataTypeAttribute&quot;&gt;
         &lt;xsd:attribute name=&quot;EvaluationMode&quot; type=&quot;EvaluationModeType&quot; default=&quot;Auto&quot; /&gt;
         &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
       &lt;/xsd:extension&gt;
     &lt;/xsd:simpleContent&gt;
   &lt;/xsd:complexType&gt;
   &lt;xsd:simpleType name=&quot;EvaluationModeType&quot;&gt;
     &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
       &lt;xsd:enumeration value=&quot;Auto&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Constant&quot; /&gt;
     &lt;/xsd:restriction&gt;
  &lt;/xsd:simpleType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>