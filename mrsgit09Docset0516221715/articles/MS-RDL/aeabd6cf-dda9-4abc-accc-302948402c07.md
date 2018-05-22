<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.329.3 Filter.Operator</title>
        <xml>
            <mshelp:toctitle title="2.329.3 Filter.Operator"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Filter.Operator"></mshelp:rltitle>
            <mshelp:keyword index="A" term="aeabd6cf-dda9-4abc-accc-302948402c07"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="aeabd6cf-dda9-4abc-accc-302948402c07"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Filter.Operator" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.329.3 Filter.Operator</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Filter.Operator</b> element specifies an operator to
use to compare the values of <a href="6cfe60b1-d7e0-4e1e-807e-0ca41147cc29.htm">Filter.FilterExpression</a>
and <a href="6bd82e79-e154-4159-94ef-b950fbba402d.htm">FilterValues</a>. The <b>Filter.Operator</b>
element MUST be specified. The value of this element MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.htm">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) that is one of the following:</p>

<p><b>Equal</b>: Specifies an equality comparison.</p>

<p><b>Like</b>: Specifies a like comparison (that is, it
compares a string against a pattern).</p>

<p><b>NotEqual</b>: Specifies an inequality comparison.</p>

<p><b>GreaterThan</b>: Specifies a comparison to
determine whether the <b>Filter.FilterExpression</b> value is greater than the <b>FilterValues</b>
values.</p>

<p><b>GreaterThanOrEqual</b>: Specifies a comparison to
determine whether the <b>Filter.FilterExpression</b> value is greater than or
equal to the <b>FilterValues</b> values.</p>

<p><b>LessThan</b>: Specifies a comparison to determine
whether the <b>Filter.FilterExpression</b> value is less than the <b>FilterValues</b>
values.</p>

<p><b>LessThanOrEqual</b>: Specifies a comparison to
determine whether the <b>Filter.FilterExpression</b> value is less than or
equal to the <b>FilterValues</b> values.</p>

<p><b>TopN</b>: Specifies whether the <b>Filter.FilterExpression</b>
value is within the top <i>N</i> data values, where <i>N</i> is specified by <a href="b51efba3-fe3e-4d6c-a95b-c047cca07efb.htm">FilterValues.FilterValue</a>. </p>

<p><b>BottomN</b>: Specifies whether the <b>Filter.FilterExpression</b>
value is within the bottom <i>N</i> data values, where <i>N</i> is specified by
<b>FilterValues.FilterValue</b>.</p>

<p><b>TopPercent</b>: Specifies whether the <b>Filter.FilterExpression</b>
value is within the top <i>N</i> percent of data values, where <i>N</i> is
specified by <b>FilterValues.FilterValue</b>.</p>

<p><b>BottomPercent</b>: Specifies whether the <b>Filter.FilterExpression</b>
value is within the bottom <i>N</i> percent of data values, where <i>N</i> is
specified by <b>FilterValues.FilterValue</b>.</p>

<p><b>In</b>: Specifies whether the value of <b>Filter.FilterExpression</b>
is equal to any <b>FilterValues.FilterValue</b> instances.</p>

<p><b>Between</b>: Specifies whether the value of <b>Filter.FilterExpression</b>
is between the values of two <b>FilterValues.FilterValue</b> instances.</p>

<p>The <b>TopN</b>, <b>BottomN</b>, <b>TopPercent</b>, and <b>BottomPercent</b>
operators SHOULD include ties in the resulting data. String comparisons within
filters SHOULD be locale-dependent. The NULL constant is equal to itself. </p>

<p>The <b>TopPercent</b> and <b>BottomPercent</b> operators
SHOULD round up and down, respectively, if the percentage that is specified
would result in a partial item being included (for example, if the Top 25% of
13 items is four items and the Bottom 75% is nine items). If the value of the <b>Filter.Operator</b>
element is &quot;In&quot;, multi-value report parameters that have the <a href="c21237a1-8237-4538-a105-1f760242de1d.htm">ReportParameter.MultiValue</a>
element specified with a value of true MUST be supported and treated as
multiple <b>FilterValue</b> instances. </p>

<p>In the following example, if &quot;Cities&quot; is a
multi-value parameter for a <a href="c0f6a66a-1055-4f4d-b1e7-4fc47b588ed2.htm">Filter</a>
that references &quot;Cities&quot; within any <b>FilterValues.FilterValue</b>
elements, the following RDL:</p>

<dl>
<dd>
<div><pre> &lt;FilterValues&gt;
    &lt;FilterValue&gt;=Parameters!Cities.Value&lt;/FilterValue&gt;
 &lt;/FilterValues&gt;
</pre></div>
</dd></dl>

<p>MUST be equivalent to the following RDL:</p>

<dl>
<dd>
<div><pre> &lt;FilterValues&gt;
    &lt;FilterValue&gt;=Parameters!Cities.Value[0]&lt;/FilterValue&gt;
    &lt;FilterValue&gt;=Parameters!Cities.Value[1]&lt;/FilterValue&gt;
    […]
 &lt;/FilterValues&gt;
</pre></div>
</dd></dl>

<p>Following is the parent element of the <b>Filter.Operator</b>
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
  <p>Filter</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Filter.Operator</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Operator&quot;&gt;
   &lt;xsd:simpleType&gt;
     &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
       &lt;xsd:enumeration value=&quot;Equal&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Like&quot; /&gt;
       &lt;xsd:enumeration value=&quot;NotEqual&quot; /&gt;
       &lt;xsd:enumeration value=&quot;GreaterThan&quot; /&gt;
       &lt;xsd:enumeration value=&quot;GreaterThanOrEqual&quot; /&gt;
       &lt;xsd:enumeration value=&quot;LessThan&quot; /&gt;
       &lt;xsd:enumeration value=&quot;LessThanOrEqual&quot; /&gt;
       &lt;xsd:enumeration value=&quot;TopN&quot; /&gt;
       &lt;xsd:enumeration value=&quot;BottomN&quot; /&gt;
       &lt;xsd:enumeration value=&quot;TopPercent&quot; /&gt;
       &lt;xsd:enumeration value=&quot;BottomPercent&quot; /&gt;
       &lt;xsd:enumeration value=&quot;In&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Between&quot; /&gt;
     &lt;/xsd:restriction&gt;
   &lt;/xsd:simpleType&gt;
 &lt;/xsd:element&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>