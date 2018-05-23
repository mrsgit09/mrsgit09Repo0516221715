<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.203.5 StateIndicator.Left</title>
        <xml>
            <mshelp:toctitle title="2.203.5 StateIndicator.Left"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: StateIndicator.Left"></mshelp:rltitle>
            <mshelp:keyword index="A" term="bb597b05-fcfe-4cea-9dba-d5afdd494568"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="bb597b05-fcfe-4cea-9dba-d5afdd494568"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: StateIndicator.Left" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.203.5 StateIndicator.Left</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>StateIndicator.Left</b> element specifies the distance
from the left as a percentage of the <a href="ee5193d7-d30d-494d-93cd-ae8ed0a570bf.md">StateIndicator.ParentItem</a>.
If <b>StateIndicator.ParentItem</b> is not specified, the value of the <b>StateIndicator.Left</b>
element is interpreted relative to the left of the <a href="f01744d3-79fa-4f30-94bf-a1ffa6bde2ac.md">GaugePanel</a>.</p>

<p>The <b>StateIndicator.Left</b> element is optional. This
element is ignored if it is present in any schema version prior to
RDL 2010/01. However, its data type is validated, and the value MUST be a <a href="c7d0946f-992e-4abc-a304-09b53e030692.md">Float</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.4) or an expression that evaluates to a <b>Float</b>. If the <a href="f9d6ec8d-393e-41b9-9ba6-e13c09aff56c.md">GaugePanel.AutoLayout</a>
property for the <b>StateIndicator.Left</b> element’s parent <b>GaugePanel</b>
element is set to true, the <b>StateIndicator.Left</b> element is ignored. If
the <b>StateIndicator.Left</b> element is not present, its value is interpreted
as 0.</p>

<p>The following is the parent element of the <b>StateIndicator.Left</b>
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
  <p><a href="a2711217-7047-4b0a-86d1-d01b5479e2cb.md">StateIndicator</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>StateIndicator.Left</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Left&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>