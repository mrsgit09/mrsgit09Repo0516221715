<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.68.22 Table.DataSetName</title>
        <xml>
            <mshelp:toctitle title="2.68.22 Table.DataSetName"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Table.DataSetName"></mshelp:rltitle>
            <mshelp:keyword index="A" term="b6c3ce4e-4d4e-404a-bac1-7bbc5b12bcf4"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="b6c3ce4e-4d4e-404a-bac1-7bbc5b12bcf4"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Table.DataSetName" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.68.22 Table.DataSetName</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.html"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.html"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>Table.DataSetName</b> element specifies the name of
the <a href="a14782b0-2e2f-4305-83a3-3de3fd750b6a.html">DataSet</a> to use to
bind data to a <a href="660db744-699e-4ca3-a2d6-a5cab4bcf9b0.html">Table</a>.
This element is optional. If this element is present, its value MUST be a
case-sensitive <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_cb2ad790-a668-429f-84fa-f3dd67517e9b">CLS-compliant
identifier</a> <a href="https://go.microsoft.com/fwlink/?LinkId=147989">[UTR15]</a>
that is the value of the <b>Name</b> attribute of a <b>DataSet</b> element
contained within the <a href="6bbaafec-020b-406c-b4e7-5e4318b616cb.html">Report</a>.</p>

<p>This element MUST be specified if both of the following
statements are true:</p>

<ul><li><p><span><span> 
</span></span>The table is not contained within another data region.</p>

</li><li><p><span><span> 
</span></span>There is more than one dataset specified for the report.</p>

</li></ul><p>This element is ignored for a table that is contained within
another data region. A table MUST NOT be specified in a report if there is no <b>DataSet</b>
element specified in the containing report. If this element is not present, its
value is interpreted as the value of the <b>DataSetName</b> of the first
ancestor data region the table is contained within, or the name of the single <b>DataSet</b>
specified for the report.</p>

<p>Following is the parent element of the <b>Table.DataSetName</b>
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
  <p>Table</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Table.DataSetName</b>
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