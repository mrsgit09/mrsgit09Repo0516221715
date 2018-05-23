<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.49.9 Matrix.Label</title>
        <xml>
            <mshelp:toctitle title="2.49.9 Matrix.Label"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Matrix.Label"></mshelp:rltitle>
            <mshelp:keyword index="A" term="fd6f5eea-d8ed-4b15-a34e-f3dba38fec70"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="fd6f5eea-d8ed-4b15-a34e-f3dba38fec70"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Matrix.Label" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.49.9 Matrix.Label</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.html"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.html"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>Matrix.Label</b> element specifies a document map
label to identify a <a href="25419c0a-c7c6-43d7-8ca5-1af842666dcb.html">Matrix</a>
within the rendered <a href="6bbaafec-020b-406c-b4e7-5e4318b616cb.html">Report</a>.</p>

<p>This element is optional. If <b>Matrix.Label</b> is
specified, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a> or an expression
that evaluates to a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_a3af3eaf-64b7-499b-a95f-193cd4c27812">Variant</a>.
If the expression returns NULL, no item is added to the document map. This
element is ignored if the <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_32295443-a111-4846-955d-a3f5964726bb">matrix</a>
is contained within a page header or page footer.</p>

<p>Following is the parent element of the <b>Matrix.Label</b>
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
  <p>Matrix</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Matrix.Label</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Label&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>