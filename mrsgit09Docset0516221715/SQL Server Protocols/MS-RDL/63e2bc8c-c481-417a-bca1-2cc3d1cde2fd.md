<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.202 StateIndicators</title>
        <xml>
            <mshelp:toctitle title="2.202 StateIndicators"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: StateIndicators"></mshelp:rltitle>
            <mshelp:keyword index="A" term="63e2bc8c-c481-417a-bca1-2cc3d1cde2fd"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="63e2bc8c-c481-417a-bca1-2cc3d1cde2fd"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: StateIndicators" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.202 StateIndicators</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>StateIndicators</b> element is ignored in any schema
version prior to RDL 2010/01.</p>

<p>The following are the parent and child elements for the <b>StateIndicators</b>
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
  <p><a href="f01744d3-79fa-4f30-94bf-a1ffa6bde2ac.md">GaugePanel</a></p>
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
  <p><a href="c7ef52b9-bf7e-4062-a953-4ff59e42d267.md">StateIndicators.StateIndicator</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>StateIndicators</b>
element in RDL 2008/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;StateIndicatorsType&quot;&gt;
   &lt;xsd:sequence&gt;
     &lt;xsd:element name=&quot;StateIndicator&quot; type=&quot;StateIndicatorType&quot; minOccurs=&quot;1&quot; 
                  maxOccurs=&quot;unbounded&quot; /&gt;
   &lt;/xsd:sequence&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>StateIndicators</b>
element in RDL 2010/01 and <a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md">RDL 2016/01</a>.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;StateIndicatorsType&quot;&gt;
   &lt;xsd:sequence&gt;
     &lt;xsd:element name=&quot;StateIndicator&quot; type=&quot;StateIndicatorType&quot; minOccurs=&quot;1&quot; 
                  maxOccurs=&quot;unbounded&quot; /&gt;
   &lt;/xsd:sequence&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>