<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.3.98 LayoutDirection</title>
        <xml>
            <mshelp:toctitle title="2.3.98 LayoutDirection"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: LayoutDirection"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8a4b0caa-0ddd-45d0-a9cd-6ead08e8a592"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8a4b0caa-0ddd-45d0-a9cd-6ead08e8a592"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: LayoutDirection" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.3.98 LayoutDirection</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>LayoutDirection</b> property specifies the direction
of the layout of <a href="f8ea94d9-d2b6-4d7f-8dc4-59faa3a98b93.htm">Tablix</a>
columns. If this property is specified, it MUST be part of the <a href="2a40ce87-0857-4776-ac72-ba5668c8340a.htm">TablixMeasurements</a> record.
If this property is not specified, the default value is used.</p>

<dl>
<dd>
<div><pre> LayoutDirection = layoutDirectionStart layoutDirectionValue
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
  <p>layoutDirectionStart</p>
  </td>
  <td colspan="8">
  <p>layoutDirectionValue</p>
  </td>
  
 </tr>
</table>

<p><b>layoutDirectionStart (1 byte): </b>A byte that
specifies the start of the <b>LayoutDirection</b> property. The value of the <b>layoutDirectionStart</b>
field MUST be the following value.</p>

<dl>
<dd>
<table>
 <thead>
  <tr>
   <th>
   <p>Value</p>
   </th>
   <th>
   <p>Parent</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>0x03</p>
  </td>
  <td>
  <p>TablixMeasurements</p>
  </td>
 </tr>
</table>
</dd></dl>

<p><b>layoutDirectionValue (1 byte): </b>A byte that
specifies the layout direction of <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.htm#gt_f9f5d4be-2a9e-4556-90f6-d4ed1678f0b4">tablix</a> columns. The value
of the <b>layoutDirectionValue</b> field MUST be defined by the <a href="35c3d4dd-dc15-4e61-a4d9-7b45896a7ab6.htm">Directions</a> <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.htm#gt_846463b5-421c-4d6b-8d82-79d44db666fa">enumeration</a>. The default
value is 0x00.</p>


                </div>
            </div>
        </div>
    </body>
</html>