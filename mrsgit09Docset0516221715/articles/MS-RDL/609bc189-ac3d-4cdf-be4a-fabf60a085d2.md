<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.11.9 Image.Height</title>
        <xml>
            <mshelp:toctitle title="2.11.9 Image.Height"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Image.Height"></mshelp:rltitle>
            <mshelp:keyword index="A" term="609bc189-ac3d-4cdf-be4a-fabf60a085d2"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="609bc189-ac3d-4cdf-be4a-fabf60a085d2"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Image.Height" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.11.9 Image.Height</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Image.Height</b> element specifies the height of an <a href="63e1e5ab-7c49-4f62-8dbd-62d85de2b153.md">Image</a>. This element is
optional. If this element is present, its value MUST be an <a href="b40c092e-4fe5-4f7b-a0bf-c98df1361c90.md">RdlSize</a>. If this element
is not present, its value is interpreted as the height of the image's
container, such as a <b>Rectangle</b> or <b>Body</b>, minus the value of the <a href="87b4ca54-7e3c-4fb6-bf62-9e24b7dd36fd.md">Image.Top</a> element, if
specified.</p>

<p>Following is the parent element of the <b>Image.Height</b>
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
  <p>Image</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Image.Height</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Height&quot; type=&quot;SizeType&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>