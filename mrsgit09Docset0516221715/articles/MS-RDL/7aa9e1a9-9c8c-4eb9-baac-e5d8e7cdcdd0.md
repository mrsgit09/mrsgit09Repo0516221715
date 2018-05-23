<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.47.2 LabelData.Key</title>
        <xml>
            <mshelp:toctitle title="2.47.2 LabelData.Key"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: LabelData.Key"></mshelp:rltitle>
            <mshelp:keyword index="A" term="7aa9e1a9-9c8c-4eb9-baac-e5d8e7cdcdd0"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="7aa9e1a9-9c8c-4eb9-baac-e5d8e7cdcdd0"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: LabelData.Key" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.47.2 LabelData.Key</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.html"><b><i>RDL 2011/01</i></b></a></p>

<p>The <b>LabelData.Key</b> element specifies the name of the <a href="a14782b0-2e2f-4305-83a3-3de3fd750b6a.html">DataSet</a> Field to be
matched with a band (<a href="e42fb86e-799a-4202-8845-ac38831efccb.html">Tablix</a>)
<a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_75bd4c80-aee7-4a88-bfb7-2228acc3ffe6">group expression</a> value.
The <b>LabelData.Key</b> element is optional. If this element is specified, its
value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.html">String</a>
(<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a>
section 3.2.1) that is one of the <a href="6da34dff-0fdf-4ae2-92dc-2af0ece382bc.html">Field.Name</a> attribute
values of the <b>DataSet</b> for slider metadata.</p>

<p>The following is the parent element of the <b>LabelData.Key</b>
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
  <p><a href="7303c2e5-ce21-4b95-a9ee-a25edc46c34a.html">LabelData</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>LabelData.Key</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Key&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;/&gt;
  
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>