<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.330.1 FilterValues.FilterValue</title>
        <xml>
            <mshelp:toctitle title="2.330.1 FilterValues.FilterValue"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: FilterValues.FilterValue"></mshelp:rltitle>
            <mshelp:keyword index="A" term="b51efba3-fe3e-4d6c-a95b-c047cca07efb"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="b51efba3-fe3e-4d6c-a95b-c047cca07efb"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: FilterValues.FilterValue" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.330.1 FilterValues.FilterValue</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>FilterValues.FilterValue</b> element specifies a
value to compare to the value of the <a href="6cfe60b1-d7e0-4e1e-807e-0ca41147cc29.html">Filter.FilterExpression</a>
element by using the <a href="aeabd6cf-dda9-4abc-accc-302948402c07.html">Filter.Operator</a>
element.</p>

<p>If <b>Filter.Operator</b> is not set to &quot;In&quot; or
&quot;Between&quot;, there MUST be exactly one <b>FilterValues.FilterValue</b>
element. </p>

<p>If <b>Filter.Operator</b> is set to &quot;TopN&quot; or
&quot;BottomN&quot;, the value of the <b>FilterValues.FilterValue</b> element
MUST be an <a href="176fbb59-c3e2-430c-b1bb-37fd15df813e.html">Integer</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.3.17) or an expression that evaluates to an <b>Integer</b>. </p>

<p>If <b>Filter.Operator</b> is set to &quot;TopPercent&quot;
or &quot;BottomPercent&quot;, the value of the <b>FilterValues.FilterValue</b>
element MUST be a <a href="c7d0946f-992e-4abc-a304-09b53e030692.html">Float</a>
([XMLSCHEMA2] section 3.2.4) or an expression that evaluates to a <b>Float</b>.
</p>

<p>If <b>Filter.Operator</b> is set to &quot;Between&quot;,
there MUST be exactly two <b>FilterValue</b> elements.</p>

<p>The following are the parent element and attribute of the <b>FilterValues.FilterValue</b>
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
  <p><a href="6bd82e79-e154-4159-94ef-b950fbba402d.html">FilterValues</a></p>
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
  <p><a href="f29f2111-e458-4aac-aabd-3086ad4d7acc.html">FilterValues.FilterValue.DataType</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>FilterValues.FilterValue</b>
element in <a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.html">RDL 2003/10</a><span> </span>and <a href="3ebe2912-4958-4832-b391-cad1f5e13338.html">RDL 2005/01</a>.</p>

<dl>
<dd>
<div><pre>     &lt;xsd:element name=&quot;FilterValue&quot; type=&quot;xsd:string&quot; 
                  maxOccurs=&quot;unbounded&quot; /&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>FilterValues.FilterValue</b>
element in <a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html">RDL 2008/01</a>,
<a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html">RDL 2010/01</a>, and <a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html">RDL 2016/01</a>.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;FilterValue&quot; type=&quot;StringWithDataTypeAttribute&quot; maxOccurs=&quot;unbounded&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>