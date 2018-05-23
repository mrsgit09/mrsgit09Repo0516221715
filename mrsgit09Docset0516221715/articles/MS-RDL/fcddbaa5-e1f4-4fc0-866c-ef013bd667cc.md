<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.87.23 Chart.DataElementOutput</title>
        <xml>
            <mshelp:toctitle title="2.87.23 Chart.DataElementOutput"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Chart.DataElementOutput"></mshelp:rltitle>
            <mshelp:keyword index="A" term="fcddbaa5-e1f4-4fc0-866c-ef013bd667cc"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="fcddbaa5-e1f4-4fc0-866c-ef013bd667cc"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Chart.DataElementOutput" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.87.23 Chart.DataElementOutput</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Chart.DataElementOutput</b> element specifies whether
an item appears in a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_9069c206-b9e9-4374-a7ee-50faf5def25b">data
rendering</a>. This element is optional. If the <b>Chart.DataElementOutput</b>
element is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) that is one of the following:</p>

<p><b>Output</b>: Specifies that the item appears in the
data rendering output.</p>

<p><b>NoOutput</b>: Specifies that the item does not
appear in the data rendering output.</p>

<p><b>ContentsOnly</b>: Specifies that the item itself
does not appear in the data rendering output, but that the contents of the item
appear in the data rendering output.</p>

<p><b>Auto</b> (default): Specifies that the item does
not appear in the data rendering output if, in <a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.md">RDL 2003/10</a> and <a href="3ebe2912-4958-4832-b391-cad1f5e13338.md">RDL 2005/01</a>, the <a href="f3877c9b-4a9b-4fd5-a680-90f763d513b5.md">Chart.Visibility</a> element
has its Hidden property set to true or if, in <a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md">RDL 2008/01</a>, <a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md">RDL 2010/01</a>, and <a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md">RDL 2016/01</a>, the
value of the grandchild <a href="7b643798-b8f4-4f1d-8f77-7e3626e58270.md">Visibility.Hidden</a>
element of the <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.md">Chart</a>
element is present and is set to true. Otherwise, the value of the <b>Chart.DataElementOutput</b>
element is interpreted as &quot;Output&quot;.</p>

<p>If the <b>Chart.DataElementOutput</b> element is not
present, its value is interpreted as &quot;Auto&quot;.</p>

<p>Following is the parent element of the <b>Chart.DataElementOutput</b>
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
  <p>Chart</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Chart.DataElementOutput</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;DataElementOutput&quot; minOccurs=&quot;0&quot;&gt;
   &lt;xsd:simpleType&gt;
     &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
       &lt;xsd:enumeration value=&quot;Output&quot; /&gt;
       &lt;xsd:enumeration value=&quot;NoOutput&quot; /&gt;
       &lt;xsd:enumeration value=&quot;ContentsOnly&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Auto&quot; /&gt;
     &lt;/xsd:restriction&gt;
   &lt;/xsd:simpleType&gt;
 &lt;/xsd:element&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>