<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.87.24 Chart.DataSetName</title>
        <xml>
            <mshelp:toctitle title="2.87.24 Chart.DataSetName"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Chart.DataSetName"></mshelp:rltitle>
            <mshelp:keyword index="A" term="eb1ed7cf-bc15-41ff-9011-cec16efdf6b6"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="eb1ed7cf-bc15-41ff-9011-cec16efdf6b6"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Chart.DataSetName" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.87.24 Chart.DataSetName</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Chart.DataSetName</b> element specifies the name of
the <a href="a14782b0-2e2f-4305-83a3-3de3fd750b6a.html">DataSet</a> to use for
a data region. This element is optional. If this element is present, its value
MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1). </p>

<p>The <b>Chart.DataSetName</b> element MUST be specified if
both of the following statements are true:</p>

<ul><li><p><span><span> 
</span></span>The <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.html">Chart</a>
is not contained within another data region.</p>

</li><li><p><span><span> 
</span></span>More than one dataset is specified for the <a href="6bbaafec-020b-406c-b4e7-5e4318b616cb.html">Report</a>.</p>

</li></ul><p>If no dataset is specified for the containing report, the
chart does not render.</p>

<p>In <a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html">RDL 2008/01</a>,
<a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html">RDL 2010/01</a>, and <a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html">RDL 2016/01</a>, if the <b>Chart</b>
has an ancestor, the value of the <b>Chart.DataSetName</b> element is
interpreted as the <b>DataSet.Name</b> for the containing scope (<b>DataRegion</b>,
<a href="dbfff811-1be7-4e8b-a5d2-6cc522317fbe.html">Group</a>, or <b>Cell</b>).<a id="Appendix_A_Target_22"></a><a href="1fe5fd87-2de5-4b2c-b762-5a4fd1373621.html#Appendix_A_22" aria-label="Product behavior note 22">&lt;22&gt;</a></p>

<p>Following is the parent element of the <b>Chart.DataSetName</b>
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
  <p>Chart</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Chart.DataSetName</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;DataSetName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>