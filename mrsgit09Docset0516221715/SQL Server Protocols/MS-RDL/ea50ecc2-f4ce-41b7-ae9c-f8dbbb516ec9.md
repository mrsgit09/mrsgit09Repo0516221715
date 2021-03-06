<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.137 ChartSeriesCollection</title>
        <xml>
            <mshelp:toctitle title="2.137 ChartSeriesCollection"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: ChartSeriesCollection"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ea50ecc2-f4ce-41b7-ae9c-f8dbbb516ec9"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ea50ecc2-f4ce-41b7-ae9c-f8dbbb516ec9"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: ChartSeriesCollection" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.137 ChartSeriesCollection</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>ChartSeriesCollection</b> element specifies a list of
<a href="aee11573-3fcf-4365-938b-e6c8ceece6e1.md">ChartSeries</a>.</p>

<p>The following are the parent and child elements of the <b>ChartSeriesCollection</b>
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
  <p><a href="1aee64b7-3829-41b6-b546-544f42867119.md">ChartData</a></p>
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
  <p><a href="3cd0ca19-a6b4-44ad-9cd7-f24d3ac6354a.md">ChartSeriesCollection.ChartSeries</a>
  </p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>ChartSeriesCollection</b>
element in RDL 2008/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;ChartSeriesCollectionType&quot;&gt;
   &lt;xsd:sequence maxOccurs=&quot;unbounded&quot; minOccurs=&quot;1&quot;&gt;
     &lt;xsd:element name=&quot;ChartSeries&quot; type=&quot;ChartSeriesType&quot; minOccurs=&quot;1&quot; 
                  maxOccurs=&quot;unbounded&quot; /&gt;
   &lt;/xsd:sequence&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>ChartSeriesCollection</b>
element in RDL 2010/01 and RDL 2016/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;ChartSeriesCollectionType&quot;&gt;
   &lt;xsd:sequence maxOccurs=&quot;unbounded&quot; minOccurs=&quot;1&quot;&gt;
     &lt;xsd:element name=&quot;ChartSeries&quot; type=&quot;ChartSeriesType&quot; minOccurs=&quot;1&quot; 
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