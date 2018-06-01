<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.3.24 Columns</title>
        <xml>
            <mshelp:toctitle title="2.3.24 Columns"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: Columns"></mshelp:rltitle>
            <mshelp:keyword index="A" term="89db4ec2-67d0-4fae-a423-1bdb8aa9d2ea"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="89db4ec2-67d0-4fae-a423-1bdb8aa9d2ea"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: Columns" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.3.24 Columns</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Columns</b> property specifies the number of columns
a page contains. If this property is specified, it MUST be part of a <a href="0b56e16b-0d77-4cad-83a4-1ba0c046a35c.md">PageProperties</a> record. If
the <b>Columns</b> property is not specified, the default value is
used.           </p>

<dl>
<dd>
<div><pre> Columns = columnsStart columnsValue
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
  <p>columnsStart</p>
  </td>
  <td colspan="24">
  <p>columnsValue</p>
  </td>
 </tr>
 <tr>
  <td colspan="8">
  <p>...</p>
  </td>
  
 </tr>
</table>

<p><b>columnsStart (1 byte): </b>A byte that specifies
the start of the <b>Columns</b> property. The value of the <b>columnStart</b>
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
  <p>0x17</p>
  </td>
  <td>
  <p>PageProperties</p>
  </td>
 </tr>
</table>
</dd></dl>

<p><b>columnsValue (4 bytes): </b>A signed integer that
specifies the number of columns a page contains. The default value is
0x00000000.</p>


                </div>
            </div>
        </div>
    </body>
</html>