<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.151.12 ChartLegend.HeaderSeparator</title>
        <xml>
            <mshelp:toctitle title="2.151.12 ChartLegend.HeaderSeparator"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: ChartLegend.HeaderSeparator"></mshelp:rltitle>
            <mshelp:keyword index="A" term="e7f6deaf-c19b-4072-bce2-861cedeae131"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="e7f6deaf-c19b-4072-bce2-861cedeae131"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: ChartLegend.HeaderSeparator" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.151.12 ChartLegend.HeaderSeparator</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>ChartLegend.HeaderSeparator</b> element specifies the
type of separator to use for the chart legend header in a <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.md">Chart</a>. This element is
optional. </p>

<p>If the <b>ChartLegend.HeaderSeparator</b> element is
present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a>
(<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a>
section 3.2.1) or an expression that evaluates to a <b>String</b>. The value of
this element MUST be one of the following or an expression that evaluates to
one of the following:</p>

<p><b>None:</b> Specifies no separator.</p>

<p><b>Line:</b> Specifies to separate with a line.</p>

<p><b>ThickLine:</b> Specifies to separate with thick
line.</p>

<p><b>DoubleLine:</b> Specifies to separate with a
double line.</p>

<p><b>DashLine:</b> Specifies to separate with a dashed
line.</p>

<p><b>DotLine:</b> Specifies to separate with a dotted
line.</p>

<p><b>GradientLine:</b> Specifies to separate with a
gradient line.</p>

<p><b>ThickGradientLine:</b> Specifies to separate with
a thick gradient line.</p>

<p>If the <b>ChartLegend.HeaderSeparator</b> element is not
present, its value is interpreted as &quot;None&quot;.</p>

<p>Following is the parent element of the <b>ChartLegend.HeaderSeparator</b>
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
  <p><a href="68a0757c-8f1a-42b9-9473-ccedd40029fb.md">ChartLegend</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>ChartLegend.HeaderSeparator</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;HeaderSeparator&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>