<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.30.11 CellContents.Tablix</title>
        <xml>
            <mshelp:toctitle title="2.30.11 CellContents.Tablix"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: CellContents.Tablix"></mshelp:rltitle>
            <mshelp:keyword index="A" term="cb7cc349-acc7-4ecb-bb8c-a451d7ae1dfb"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="cb7cc349-acc7-4ecb-bb8c-a451d7ae1dfb"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: CellContents.Tablix" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.30.11 CellContents.Tablix</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>CellContents.Tablix</b> element specifies a <a href="e42fb86e-799a-4202-8845-ac38831efccb.md">Tablix</a> within another
tablix. This element is optional and MUST NOT be specified more than once. The <b>Top</b>,
<b>Left</b>, <b>Height</b>, and <b>Width</b> child element values are
interpreted as follows:</p>

<p><b>Top</b>: 0</p>

<p><b>Left</b>: 0</p>

<p><b>Height</b>: The same as the height of the
containing object.</p>

<p><b>Width</b>: The same as the width of the containing
object.</p>

<p>If the <b>CellContents.Tablix</b> element is specified, it
is of type <b>Tablix</b>.</p>

<p>Following is the parent element of the <b>CellContents.Tablix</b>
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
  <p><a href="43ccec32-ec37-401c-ba8a-edbfa74e42f4.md">CellContents</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>CellContents.Tablix</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Tablix&quot; type=&quot;TablixType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>