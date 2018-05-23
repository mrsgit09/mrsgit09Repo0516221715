<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.242.3 MapMarkerTemplate.DataElementName</title>
        <xml>
            <mshelp:toctitle title="2.242.3 MapMarkerTemplate.DataElementName"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapMarkerTemplate.DataElementName"></mshelp:rltitle>
            <mshelp:keyword index="A" term="9cd5dfd1-be3f-45a0-bbd3-ad46780fcf56"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="9cd5dfd1-be3f-45a0-bbd3-ad46780fcf56"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapMarkerTemplate.DataElementName" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.242.3 MapMarkerTemplate.DataElementName</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapMarkerTemplate.DataElementName</b> element
specifies a name for the <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_3ff4ae5f-17e5-4291-ad80-f2a312119b0a">marker
template</a> to use for a data element or attribute. This element is optional.
If this element is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) that is a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_cb2ad790-a668-429f-84fa-f3dd67517e9b">CLS-compliant
identifier</a> <a href="https://go.microsoft.com/fwlink/?LinkId=147989">[UTR15]</a>.
If this element is not present, its value is interpreted as
&quot;MapDataRow&quot;.</p>

<p>Following is the parent element of the <b>MapMarkerTemplate.DataElementName</b>
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
  <p><a href="22055a42-2ec0-48cd-893f-f7bd717efc7a.html">MapMarkerTemplate</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapMarkerTemplate.DataElementName</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;DataElementName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
  
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>