<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.39 ImageData</title>
        <xml>
            <mshelp:toctitle title="2.2.39 ImageData"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: ImageData"></mshelp:rltitle>
            <mshelp:keyword index="A" term="2a8aaaa7-3ccf-4f0a-93c6-d99c73ed40fe"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="2a8aaaa7-3ccf-4f0a-93c6-d99c73ed40fe"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: ImageData" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.39 ImageData</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>ImageData</b> property specifies a structure that
defines the content for an <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.htm#gt_d6b55d1e-aea6-4b7e-a23d-c0de845e0b50">image</a>.
If this property is specified, it MUST be part of one of the following records:</p>

<ul><li><p><span><span> 
</span></span><a href="1b93acb6-ccb8-494f-abe9-797e9d3ab199.htm">ImageDataProperties.InlineSharedImageDataProperties</a></p>

</li><li><p><span><span> 
</span></span><a href="cd824380-615e-4259-9193-320c0992eb47.htm">ImageDataProperties.NonSharedImageDataProperties</a>          
</p>

<div><pre> ImageData = imageDataStart count imageDataContent
</pre></div>

</li></ul><table>
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
  <p>imageDataStart</p>
  </td>
  <td colspan="24">
  <p>count</p>
  </td>
 </tr>
 <tr>
  <td colspan="8">
  <p>...</p>
  </td>
  <td colspan="24">
  <p>imageDataContents
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
</table>

<p><b>imageDataStart (1 byte): </b>A byte that specifies
the start of the <b>ImageData</b> record. The value of the <b>imageDataStart</b>
field MUST be 0x02.</p>

<p><b>count (4 bytes): </b>A signed integer that
specifies the number of bytes that comprise the image content.</p>

<p><b>imageDataContents (variable): </b>An array of
bytes that comprise the image. The number of bytes in the array MUST be equal
to the value of the <b>count</b> field.</p>


                </div>
            </div>
        </div>
    </body>
</html>