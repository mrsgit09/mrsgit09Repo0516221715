<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.87.1 Chart.Name</title>
        <xml>
            <mshelp:toctitle title="2.87.1 Chart.Name"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Chart.Name"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ec991d49-e2ee-4e96-abfa-e3ff8c3f699a"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ec991d49-e2ee-4e96-abfa-e3ff8c3f699a"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Chart.Name" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.87.1 Chart.Name</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Chart.Name</b> attribute specifies the name of a <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.md">Chart</a>. This attribute MUST
be specified. The value of the <b>Chart.Name</b> attribute MUST be a
case-sensitive <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_cb2ad790-a668-429f-84fa-f3dd67517e9b">CLS-compliant
identifier</a> <a href="https://go.microsoft.com/fwlink/?LinkId=147989">[UTR15]</a>
that is unique among data regions, groups, and scope names in the <a href="6bbaafec-020b-406c-b4e7-5e4318b616cb.md">Report</a>.</p>

<p>Following is the parent element of the <b>Chart.Name</b>
attribute.</p>

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

<p>The following is the XML Schema definition of the <b>Chart.Name</b>
attribute.</p>

<dl>
<dd>
<div><pre> &lt;xsd:attribute name=&quot;Name&quot; type=&quot;xsd:normalizedString&quot; use=&quot;required&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>