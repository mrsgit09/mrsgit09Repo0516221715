<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.22.21 Tablix.NoRowsMessage</title>
        <xml>
            <mshelp:toctitle title="2.22.21 Tablix.NoRowsMessage"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Tablix.NoRowsMessage"></mshelp:rltitle>
            <mshelp:keyword index="A" term="dcff5ca3-6f2b-4f8a-b82e-b9f2d8e60d1a"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="dcff5ca3-6f2b-4f8a-b82e-b9f2d8e60d1a"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Tablix.NoRowsMessage" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.22.21 Tablix.NoRowsMessage</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>Tablix.NoRowsMessage</b> element specifies text to
render instead of the <a href="e42fb86e-799a-4202-8845-ac38831efccb.md">Tablix</a>
layout when no data is available. This element is optional and MUST NOT be
specified more than once. If this element is specified, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) or an expression that evaluates to a <b>String</b> or to null.</p>

<p>Following is the parent element of the <b>Tablix.NoRowsMessage</b>
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
  <p>Tablix</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Tablix.NoRowsMessage</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;RepeatWith&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>