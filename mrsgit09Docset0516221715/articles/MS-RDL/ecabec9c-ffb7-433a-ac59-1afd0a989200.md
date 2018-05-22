<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.208.9 Map.Height</title>
        <xml>
            <mshelp:toctitle title="2.208.9 Map.Height"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Map.Height"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ecabec9c-ffb7-433a-ac59-1afd0a989200"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ecabec9c-ffb7-433a-ac59-1afd0a989200"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Map.Height" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.208.9 Map.Height</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.htm"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>Map.Height</b> element specifies the height of a <a href="fd166dd8-6772-4507-b3f6-50a2b7cfd6ac.htm">Map</a>. This element is
optional. If this element is present, its value MUST be an <a href="b40c092e-4fe5-4f7b-a0bf-c98df1361c90.htm">RdlSize</a>. If this element
is not present, its value is interpreted as the height of the map's container
minus the value of the peer <a href="01599777-3e4c-44c7-927c-f44d34c50df0.htm">Map.Top</a>
element, if specified.</p>

<p>The following is the parent element of the <b>Map.Height</b>
element. </p>

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
  <p>Map</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Map.Height</b>
element.           </p>

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