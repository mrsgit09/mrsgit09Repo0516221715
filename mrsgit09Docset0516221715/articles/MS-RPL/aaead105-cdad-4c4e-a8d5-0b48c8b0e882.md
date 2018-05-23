<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.35 ImageDataProperties</title>
        <xml>
            <mshelp:toctitle title="2.2.35 ImageDataProperties"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: ImageDataProperties"></mshelp:rltitle>
            <mshelp:keyword index="A" term="aaead105-cdad-4c4e-a8d5-0b48c8b0e882"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="aaead105-cdad-4c4e-a8d5-0b48c8b0e882"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: ImageDataProperties" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.35 ImageDataProperties</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>ImageDataProperties</b> record specifies a collection
of properties applicable to the <a href="b6e7b187-4160-4ce2-940e-6198a7416863.html">Image</a> record and the <a href="8ac13f18-6374-424f-a690-eb9030fb3083.html">BackgroundImage</a> style
property. The <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.html#gt_8502cabb-8fac-401a-93da-3ca2ad4ddf75">parent record</a>
for the <b>ImageDataProperties</b> record MUST be one of the following:</p>

<ul><li><p><span><span> 
</span></span><a href="1b1b7882-84bb-47d4-a3d2-b020b8d23d7a.html">Image.ElementProperties.NonSharedElementProperties</a></p>

</li><li><p><span><span> 
</span></span><a href="8e7ad65c-8fc2-4a04-a02f-be9fe5b91d1e.html">Style.SharedStyleProperties</a></p>

</li><li><p><span><span> 
</span></span><a href="19ef92ab-7c9f-454f-874d-b6b04b92b117.html">Style.NonSharedStyleProperties</a>           
</p>

<div><pre> ImageDataProperties = imageStart (UseSharedImageDataProperties / InlineSharedImageDataProperties / NonSharedImageDataProperties)
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
  <p>imageStart</p>
  </td>
  <td colspan="24">
  <p>imageDataProperties
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
</table>

<p><b>imageStart (1 byte): </b>A byte that specifies the
start of the <b>ImageDataProperties</b> record. The value of the <b>imageStart</b>
field MUST be 0x2A.</p>

<p><b>imageDataProperties (variable): </b>A <a href="04bb34a6-c963-40c3-9a3f-39bf2413c125.html">UseSharedImageDataProperties</a>,
<a href="1b93acb6-ccb8-494f-abe9-797e9d3ab199.html">InlineSharedImageDataProperties</a>,
or <a href="cd824380-615e-4259-9193-320c0992eb47.html">NonSharedImageDataProperties</a>
record. When the parent record is <b>Style.SharedStyleProperties</b>, the <b>imageDataProperties</b>
MUST be <b>UseSharedImageDataProperties</b> or <b>InlineSharedImageDataProperties</b>.
The <b>imageDataProperties</b> MUST be <b>NonSharedImageDataProperties</b> when
the parent record is <b>Style.NonSharedStyleProperties</b>.</p>


                </div>
            </div>
        </div>
    </body>
</html>