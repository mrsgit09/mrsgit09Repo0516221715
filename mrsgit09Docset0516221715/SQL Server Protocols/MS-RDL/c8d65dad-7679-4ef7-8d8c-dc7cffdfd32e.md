<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.300.2 Visibility.ToggleItem</title>
        <xml>
            <mshelp:toctitle title="2.300.2 Visibility.ToggleItem"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Visibility.ToggleItem"></mshelp:rltitle>
            <mshelp:keyword index="A" term="c8d65dad-7679-4ef7-8d8c-dc7cffdfd32e"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="c8d65dad-7679-4ef7-8d8c-dc7cffdfd32e"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Visibility.ToggleItem" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.300.2 Visibility.ToggleItem</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Visibility.ToggleItem</b> element specifies the name
of a <a href="469d0032-b5ec-43d9-ab36-d3a88b9cc1f6.md">Textbox</a> that is
used to hide or unhide the containing report item. This element is optional. </p>

<p>If this element is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1). The value of this element MUST contain the name of a text box in the
same group as the containing report item or in any containing ancestor group
scope. The value of this element MUST NOT refer to a report item within <a href="afff0921-7d95-4216-8f28-635c67d539d8.md">PageSection</a> or <a href="ddc35223-1cb6-4136-823b-e72a3d12e1f9.md">PageHeaderFooter</a> element.
If the <b>Visibility.ToggleItem</b> element is not present, the appearance of
the containing report item MUST NOT be toggleable.</p>

<p>Following is the parent element of the <b>Visibility.ToggleItem</b>
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
  <p><a href="9505fbda-7f65-4874-a54a-1944059812e0.md">Visibility</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Visibility.ToggleItem</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;ToggleItem&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>