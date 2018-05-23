<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.247.4 MapMarkerImage.TransparentColor</title>
        <xml>
            <mshelp:toctitle title="2.247.4 MapMarkerImage.TransparentColor"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapMarkerImage.TransparentColor"></mshelp:rltitle>
            <mshelp:keyword index="A" term="b718e041-0cdf-4e3e-b58b-9fd5facab16b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="b718e041-0cdf-4e3e-b58b-9fd5facab16b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapMarkerImage.TransparentColor" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.247.4 MapMarkerImage.TransparentColor</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapMarkerImage.TransparentColor</b> element specifies
the color to treat as transparent in the <a href="d31b353a-74ed-40cb-9031-7c5cf39a3056.md">MapMarkerImage</a>. The <b>MapMarkerImage.TransparentColor</b>
element is optional. If this element is present, its value MUST be an <a href="b302c6a5-6023-42b1-95ed-bafcdc4b5714.md">RdlColor</a> or an expression
that evaluates to an <b>RdlColor</b>. Otherwise, the image is displayed as-is.</p>

<p>Following is the parent element of the <b>MapMarkerImage.TransparentColor</b>
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
  <p>MapMarkerImage</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapMarkerImage.TransparentColor</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;TransparentColor&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>