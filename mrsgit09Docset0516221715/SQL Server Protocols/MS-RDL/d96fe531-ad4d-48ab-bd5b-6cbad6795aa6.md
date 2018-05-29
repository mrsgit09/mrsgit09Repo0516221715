<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.49.1 Matrix.Name</title>
        <xml>
            <mshelp:toctitle title="2.49.1 Matrix.Name"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Matrix.Name"></mshelp:rltitle>
            <mshelp:keyword index="A" term="d96fe531-ad4d-48ab-bd5b-6cbad6795aa6"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="d96fe531-ad4d-48ab-bd5b-6cbad6795aa6"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Matrix.Name" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.49.1 Matrix.Name</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.md"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.md"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>Matrix.Name</b> attribute specifies a unique
identifier for a <a href="25419c0a-c7c6-43d7-8ca5-1af842666dcb.md">Matrix</a>.
This attribute MUST be specified. The value of the <b>Matrix.Name</b> attribute
MUST be a <b>NormalizedString</b> that is a case-sensitive <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_cb2ad790-a668-429f-84fa-f3dd67517e9b">CLS-compliant identifier</a> <a href="https://go.microsoft.com/fwlink/?LinkId=147989">[UTR15]</a>. This value
MUST be unique among the set of all report item and scope names.</p>

<p>Following is the parent element of the <b>Matrix.Name</b>
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
  <p>Matrix</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Matrix.Name</b>
attribute.           </p>

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