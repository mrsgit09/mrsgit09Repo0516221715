<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.19.7 TextRun.Value.DataType</title>
        <xml>
            <mshelp:toctitle title="2.19.7 TextRun.Value.DataType"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: TextRun.Value.DataType"></mshelp:rltitle>
            <mshelp:keyword index="A" term="3dd0a173-f53a-4ffd-abc7-daef0b0186c7"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="3dd0a173-f53a-4ffd-abc7-daef0b0186c7"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: TextRun.Value.DataType" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.19.7 TextRun.Value.DataType</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>TextRun.Value.DataType</b> attribute specifies the
data type of the <a href="99982bda-2dd1-4626-b8ef-da888d95f4ff.html">TextRun.Value</a>
element if the value of <b>TextRun.Value</b> is a constant. This attribute is
optional. If this attribute is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1), a <a href="4802fa14-3619-43fa-9898-3acab160a24c.html">Boolean</a>
([XMLSCHEMA2] section 3.2.2), a <a href="d3b6da93-3935-4a28-8521-268d6f7f9a9d.html">DateTime</a> ([XMLSCHEMA2]
section 3.2.7), an <a href="176fbb59-c3e2-430c-b1bb-37fd15df813e.html">Integer</a>
([XMLSCHEMA2] section 3.3.17), or a <a href="c7d0946f-992e-4abc-a304-09b53e030692.html">Float</a> ([XMLSCHEMA2]
section 3.2.4). If this attribute is not present, its value is interpreted as a
<b>String.</b></p>

<p>Following is the parent element of the <b>TextRun.Value.DataType</b>
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
  <p>TextRun.Value</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>TextRun.Value.DataType</b>
attribute.</p>

<dl>
<dd>
<div><pre> &lt;xsd:attribute name=&quot;DataType&quot; use=&quot;optional&quot;&gt;
   &lt;xsd:simpleType&gt;
     &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
       &lt;xsd:enumeration value=&quot;Boolean&quot; /&gt;
       &lt;xsd:enumeration value=&quot;DateTime&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Integer&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Float&quot; /&gt;
       &lt;xsd:enumeration value=&quot;String&quot; /&gt;
     &lt;/xsd:restriction&gt;
   &lt;/xsd:simpleType&gt;
 &lt;/xsd:attribute&gt;
            
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>