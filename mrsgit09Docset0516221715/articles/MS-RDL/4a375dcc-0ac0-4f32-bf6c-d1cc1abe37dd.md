<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.87.45 Chart.Relationship</title>
        <xml>
            <mshelp:toctitle title="2.87.45 Chart.Relationship"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Chart.Relationship"></mshelp:rltitle>
            <mshelp:keyword index="A" term="4a375dcc-0ac0-4f32-bf6c-d1cc1abe37dd"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="4a375dcc-0ac0-4f32-bf6c-d1cc1abe37dd"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Chart.Relationship" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.87.45 Chart.Relationship</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.html"><b><i>RDL 2011/01</i></b></a></p>

<p>The <b>Chart.Relationship</b> element specifies a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_2913b24a-aa1a-42cb-8b80-047821e296cb">relationship</a> to use for
correlating data in a <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.html">Chart</a>
with the data in the containing scope. The <b>Chart.Relationship</b> element is
optional and MUST NOT be specified more than once. If this element is
specified, it is of type <a href="6d1c77e5-1573-4ad6-8d2a-c507411ad94b.html">Relationship</a>.
The <b>Chart.Relationship</b> element MUST NOT be specified if there is no
containing scope.</p>

<p>This element is ignored if the data set for the <b>Chart</b>
is the same as the dataset for each containing scope.</p>

<p>Following is the parent element of the <b>Chart.Relationship</b>
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

<p>The following is the XML Schema definition of the <b>Chart.Relationship</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name =&quot;Relationship&quot; type=&quot;RelationshipType&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>