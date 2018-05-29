<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.255.8 MapTileLayer.VisibilityMode</title>
        <xml>
            <mshelp:toctitle title="2.255.8 MapTileLayer.VisibilityMode"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapTileLayer.VisibilityMode"></mshelp:rltitle>
            <mshelp:keyword index="A" term="e243ced5-ae6a-49a7-ac16-a23ccadefd00"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="e243ced5-ae6a-49a7-ac16-a23ccadefd00"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapTileLayer.VisibilityMode" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.255.8 MapTileLayer.VisibilityMode</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapTileLayer.VisibilityMode</b> element specifies the
visibility mode for a <a href="32cf17dc-a986-43fd-b7ce-8cb2429e565f.md">MapTileLayer</a>.
This element is optional. </p>

<p>If this element is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) or an expression that evaluates to a <b>String</b>. The value of this
element MUST be one of the following or an expression that evaluates to one of
the following:</p>

<p><b>Visible</b>: The layer is always visible.</p>

<p><b>Hidden</b>: The layer is always hidden.</p>

<p><b>ZoomBased</b>: The layer is shown in a zoom level
range that is defined by the <a href="4f387c09-ea9b-42c3-910c-02214c611d11.md">MapTileLayer.MaximumZoom</a>
and <a href="79ab4e34-0f4a-44a7-975b-f6d6795ce411.md">MapTileLayer.MinimumZoom</a>
elements. </p>

<p>If the <b>MapTileLayer.VisibilityMode</b> element is not
present, its value is interpreted as &quot;Visible&quot;.</p>

<p>Following is the parent element of the <b>MapTileLayer.VisibilityMode</b>
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
  <p>MapTileLayer</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapTileLayer.VisibilityMode</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;VisibilityMode&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>