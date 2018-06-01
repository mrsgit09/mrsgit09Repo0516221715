<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.10 SimpleSection</title>
        <xml>
            <mshelp:toctitle title="2.2.10 SimpleSection"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: SimpleSection"></mshelp:rltitle>
            <mshelp:keyword index="A" term="44afa6af-81c8-42aa-b6cf-77faf60ee77b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="44afa6af-81c8-42aa-b6cf-77faf60ee77b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: SimpleSection" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.10 SimpleSection</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to RPL versions 10.4, 10.5, and 10.6</i></b></p>

<p>The <b>SimpleSection</b> record specifies the structure and
layout for one report <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.md#gt_49a2b98a-d101-4889-9108-87f567e758cf">section</a>.          
</p>

<dl>
<dd>
<div><pre> SimpleSection = sectionStart SectionProperties BodyAreaElement [PageFooterElement] [PageHeaderElement] Measurements ReportElementEnd
</pre></div>
</dd></dl>

<table>
 <tr>
  <th><p><br>0</p></th>
  <th><p><br>1</p></th>
  <th><p><br>2</p></th>
  <th><p><br>3</p></th>
  <th><p><br>4</p></th>
  <th><p><br>5</p></th>
  <th><p><br>6</p></th>
  <th><p><br>7</p></th>
  <th><p><br>8</p></th>
  <th><p><br>9</p></th>
  <th><p>1<br>0</p></th>
  <th><p><br>1</p></th>
  <th><p><br>2</p></th>
  <th><p><br>3</p></th>
  <th><p><br>4</p></th>
  <th><p><br>5</p></th>
  <th><p><br>6</p></th>
  <th><p><br>7</p></th>
  <th><p><br>8</p></th>
  <th><p><br>9</p></th>
  <th><p>2<br>0</p></th>
  <th><p><br>1</p></th>
  <th><p><br>2</p></th>
  <th><p><br>3</p></th>
  <th><p><br>4</p></th>
  <th><p><br>5</p></th>
  <th><p><br>6</p></th>
  <th><p><br>7</p></th>
  <th><p><br>8</p></th>
  <th><p><br>9</p></th>
  <th><p>3<br>0</p></th>
  <th><p><br>1</p></th>
 </tr>
 <tr>
  <td colspan="8">
  <p>sectionStart</p>
  </td>
  <td colspan="24">
  <p>sectionProperties
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>bodyAreaElement
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>pageFooterElement
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>pageHeaderElement
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>measurements
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>reportElementEnd</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="16">
  <p>...</p>
  </td>
  
 </tr>
</table>

<p><b>sectionStart (1 byte): </b>A byte that specifies
the start of the <b>SimpleSection</b> record. The value of the <b>sectionStart</b>
field MUST be 0x15.</p>

<p><b>sectionProperties (variable): </b>A <a href="fcc4e2ea-6155-4426-80fa-7859b51a8394.md">SectionProperties</a> record
that specifies the properties that are applicable to the <b>SimpleSection</b>
record.</p>

<p><b>bodyAreaElement (variable): </b>A <a href="95a5d250-a0be-4523-9c2f-9c10552ab136.md">BodyAreaElement</a> record
that specifies the content of the <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.md#gt_575a1308-df3d-4439-a039-54feac0baf23">body area</a> of the <b>SimpleSection</b>
record.</p>

<p><b>pageFooterElement (variable): </b>A <a href="c6b17d7f-d30f-475d-9839-ff97d9d7d69a.md">PageFooterElement</a> record
that specifies the content of the <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.md#gt_d81590ae-1ae4-4d08-9752-093dcb419410">footer area</a> of the <b>SimpleSection</b>
record.</p>

<p><b>pageHeaderElement (variable): </b>A <a href="42322dd8-21a8-4c45-9567-393dfa424736.md">PageHeaderElement</a> record
that specifies the content of the <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.md#gt_960b6fc2-f08e-4188-9520-f9f2fb2ad4d2">header area</a> of the <b>SimpleSection</b>
record.</p>

<p><b>measurements (variable): </b>A <a href="5c5210d9-a82b-4040-8e79-800e2ee51b52.md">Measurements</a> record that
specifies the size, location, and state properties for <b>BodyAreaElement</b>, <b>PageFooterElement</b>,
and <b>PageHeaderElement</b> records. The order of the <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.md#gt_f633cdb5-cb63-4197-ad01-e7b02a745fdb">elements</a> in the <b>measurementsContent</b>
field array of the <b>Measurements</b> record MUST match the order of the <b>BodyAreaElement</b>,
<b>PageFooterElement</b>, and <b>PageHeaderElement</b> records in the <b>SimpleSection</b>
record.<a id="Appendix_A_Target_6"></a><a href="1d022514-2a2f-41df-b2f8-36f19e474fa5.md#Appendix_A_6" aria-label="Product behavior note 6">&lt;6&gt;</a></p>

<p><b>reportElementEnd (10 bytes): </b>A <a href="75f1a870-2f17-4806-b286-e67c7239e103.md">ReportElementEnd</a> record
that marks the end of the <b>SimpleSection</b> record. The <b>offset</b> field
of the <b>ReportElementEnd</b> record MUST specify the position of the <b>measurements</b>
field of the <b>SimpleSection</b> record in the RPL stream.</p>


                </div>
            </div>
        </div>
    </body>
</html>