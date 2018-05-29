<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.21 NonSharedObject</title>
        <xml>
            <mshelp:toctitle title="2.2.21 NonSharedObject"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RGDI]: NonSharedObject"></mshelp:rltitle>
            <mshelp:keyword index="A" term="dfc153fe-8b8a-4e7f-af5f-e5c6dd3ec23c"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="dfc153fe-8b8a-4e7f-af5f-e5c6dd3ec23c"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RGDI]: NonSharedObject" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.21 NonSharedObject</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>NonSharedObject</b> structure specifies an object
that can be passed as an argument to GDI+ functions. The objects are the <a href="ebbd0c06-4c68-4335-897e-577737d21387.html">Font</a>, <a href="e00f31f3-41c5-47e7-a902-d2e533892727.html">Format</a>, and <a href="b56dd4fa-9cc1-4355-9d13-cbd52f9f3b83.html">Image</a> objects; these are
specified in the <b>sharedObjectContents</b> field.</p>

<dl>
<dd>
<div><pre> NonSharedObject = notShared SharedObjectContents
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
  <p>notShared</p>
  </td>
  <td colspan="24">
  <p>sharedObjectContents
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
</table>

<p><b>notShared (1 byte): </b>A byte field that
specifies that the type of the <a href="55aa3259-66cd-4c39-9102-e056659e5a9a.html">ShareableObject</a> structure
is a <b>NonSharedObject</b> structure. The value of this field MUST be
&quot;0x00&quot;.</p>

<p><b>sharedObjectContents (variable): </b>A structure
of type <a href="aa86e07c-a153-4aea-a411-c69b4179b1ce.html">SharedObjectContents</a>
that specifies a <b>Font</b>, <b>Format</b>, or <b>Image</b> object.</p>


                </div>
            </div>
        </div>
    </body>
</html>