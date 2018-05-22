<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.182.4 PointerImage.Value</title>
        <xml>
            <mshelp:toctitle title="2.182.4 PointerImage.Value"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: PointerImage.Value"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8c17c3e6-db6f-4ee1-bf8d-ac00cd7185db"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8c17c3e6-db6f-4ee1-bf8d-ac00cd7185db"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: PointerImage.Value" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.182.4 PointerImage.Value</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.htm"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.htm"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>PointerImage.Value</b> element specifies the location
of a <a href="ecf5073e-d4ae-4742-a92f-6790140b0fe6.htm">PointerImage</a>
depending on the peer <a href="d95875ab-d00a-416b-ac72-c9fc81741720.htm">PointerImage.Source</a>
element. The <b>PointerImage.Value</b> element MUST be specified.</p>

<p>If the peer <b>PointerImage.Source</b> element is set to
&quot;External&quot; and if the value of <b>PointerImage.Value</b> is
non-empty, then the value of <b>PointerImage.Value</b> MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.htm">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) constant or an expression that evaluates to the location of an image.
This location MUST be a <a href="0e8ab873-6565-45f0-a61f-2d7da8e1ff74.htm">ReportPath</a>
or <a href="b302c6a5-6023-42b1-95ed-bafcdc4b5714.htm">RdlColor</a>.</p>

<p>If the peer <b>PointerImage.Source</b> element is set to
&quot;Embedded&quot; and if the value of <b>PointerImage.Value</b> is
non-empty, then the value of <b>PointerImage.Value</b> MUST be a <b>String</b>
constant or an expression that evaluates to the name of an <a href="6cdb345a-b502-4eee-84fd-de5ccf2a40e7.htm">EmbeddedImage</a> within the
report.</p>

<p>If the peer <b>PointerImage.Source</b> element is set to
&quot;Database&quot; and if its value is non-empty, its value MUST be an
expression that evaluates to the binary data for an image. If the <b>PointerImage.Value</b>
element has an empty value, the image MUST NOT be displayed.</p>

<p>The following is the parent element of the <b>PointerImage.Value</b>
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
  <p>PointerImage</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>PointerImage.Value</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Value&quot; type=&quot;xsd:string&quot; minOccurs=&quot;1&quot;&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>