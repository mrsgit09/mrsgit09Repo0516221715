<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.212.1 MapLocation.Left</title>
        <xml>
            <mshelp:toctitle title="2.212.1 MapLocation.Left"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapLocation.Left"></mshelp:rltitle>
            <mshelp:keyword index="A" term="9bc6db86-4b9c-47cb-bfcd-df397851e5cf"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="9bc6db86-4b9c-47cb-bfcd-df397851e5cf"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapLocation.Left" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.212.1 MapLocation.Left</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapLocation.Left</b> element specifies the distance
from the left of a <a href="55679f1a-a5b6-4b08-b284-ff6e27deedb4.md">MapViewport</a>,
a <a href="9b8a7ec3-44b5-46d8-bdca-cb99308fa1f9.md">MapTitle</a>, a <a href="71c7ce11-4e8a-433b-975a-731e089ea04f.md">MapLegend</a>, a <a href="04ab14be-9206-4c63-bc93-d68bb48ed02c.md">MapDistanceScale</a>, and a <a href="fc14b477-a2d2-4048-843d-6a19beeb30bf.md">MapColorScale</a> relative to
the containing <a href="fd166dd8-6772-4507-b3f6-50a2b7cfd6ac.md">Map</a> or <b>MapViewport</b>.
The unit of measure is specified by the <a href="1bd056ac-60fd-4854-9132-9a6c3c011729.md">MapLocation.Unit</a> element.
The <b>MapLocation.Left</b> element is optional. </p>

<p>If this element is present, its value MUST be a <a href="c7d0946f-992e-4abc-a304-09b53e030692.md">Float</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.4) or an expression that evaluates to a <b>Float</b>. If this element is
not present, its value is interpreted as 0. </p>

<p>The following is the parent element of the <b>MapLocation.Left</b>
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
  <p><a href="5888ec40-7918-47d0-9b80-4d5897124957.md">MapLocation</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapLocation.Left</b>
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