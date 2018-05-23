<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.3.16 Report.DefaultFontFamily</title>
        <xml>
            <mshelp:toctitle title="2.3.16 Report.DefaultFontFamily"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Report.DefaultFontFamily"></mshelp:rltitle>
            <mshelp:keyword index="A" term="691c71de-b19d-4eeb-a5cb-a2b0c0eca8b5"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="691c71de-b19d-4eeb-a5cb-a2b0c0eca8b5"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Report.DefaultFontFamily" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.3.16 Report.DefaultFontFamily</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>Report.DefaultFontFamily </b>element specifies the
font family that is used for all text that is rendered when an explicit font is
not defined in the <a href="f1948fe1-2937-443a-8088-62a367c155c4.html">Style.FontFamily</a>
element of any child report item.</p>

<p>The <b>Report.DefaultFontFamily</b> element is optional. If
this element is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a> (<a href="http://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1). If this element is not present, its value is interpreted as
&quot;Arial&quot;. If the value of this element is not a recognized font
family, its value is interpreted as &quot;Arial&quot;.</p>

<p>Following is the parent element of the <b>Report.DefaultFontFamily</b>
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
  <p><a href="6bbaafec-020b-406c-b4e7-5e4318b616cb.html">Report</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Report.DefaultFontFamily</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;DefaultFontFamily&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; xmlns=&quot;http://schemas.microsoft.com/sqlserver/reporting/2016/01/reportdefinition/defaultfontfamily&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>