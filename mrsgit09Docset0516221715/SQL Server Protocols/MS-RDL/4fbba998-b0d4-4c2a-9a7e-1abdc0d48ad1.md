<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.263.4 MapViewport.LeftMargin</title>
        <xml>
            <mshelp:toctitle title="2.263.4 MapViewport.LeftMargin"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: MapViewport.LeftMargin"></mshelp:rltitle>
            <mshelp:keyword index="A" term="4fbba998-b0d4-4c2a-9a7e-1abdc0d48ad1"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="4fbba998-b0d4-4c2a-9a7e-1abdc0d48ad1"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: MapViewport.LeftMargin" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.263.4 MapViewport.LeftMargin</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>MapViewport.LeftMargin</b> element specifies the left
margin for a <a href="55679f1a-a5b6-4b08-b284-ff6e27deedb4.md">MapViewport</a>
element and its parent <a href="fd166dd8-6772-4507-b3f6-50a2b7cfd6ac.md">Map</a>
element. The <b>MapViewport.LeftMargin</b> element is optional. If this element
is present, its value MUST be an <a href="b40c092e-4fe5-4f7b-a0bf-c98df1361c90.md">RdlSize</a> or an expression
that evaluates to an <b>RdlSize</b>, and its value MUST NOT be negative. If
this element is not present, its value is interpreted as 0.</p>

<p>Following is the parent element of the <b>MapViewport.LeftMargin</b>
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
  <p>MapViewport</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>MapViewport.LeftMargin</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;LeftMargin&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
  
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>