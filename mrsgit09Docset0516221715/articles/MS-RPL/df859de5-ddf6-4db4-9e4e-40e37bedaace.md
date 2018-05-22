<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.3.49 Height</title>
        <xml>
            <mshelp:toctitle title="2.3.49 Height"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: Height"></mshelp:rltitle>
            <mshelp:keyword index="A" term="df859de5-ddf6-4db4-9e4e-40e37bedaace"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="df859de5-ddf6-4db4-9e4e-40e37bedaace"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: Height" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.3.49 Height</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Height</b> property specifies the height of an <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.htm#gt_d6b55d1e-aea6-4b7e-a23d-c0de845e0b50">image</a> in pixels. If this
property is specified, it MUST be part of an <a href="1b93acb6-ccb8-494f-abe9-797e9d3ab199.htm">ImageDataProperties.InlineSharedImageDataProperties</a>
or <a href="cd824380-615e-4259-9193-320c0992eb47.htm">ImageDataProperties.NonSharedImageDataProperties</a>
record.           </p>

<dl>
<dd>
<div><pre> Height = heightStart heightValue
  
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
  <p>heightStart</p>
  </td>
  <td colspan="24">
  <p>heightValue</p>
  </td>
 </tr>
 <tr>
  <td colspan="8">
  <p>...</p>
  </td>
  
 </tr>
</table>

<p><b>heightStart (1 byte): </b>A byte that specifies
the start of the <b>Height</b> property.<a id="Appendix_A_Target_32"></a><a href="1d022514-2a2f-41df-b2f8-36f19e474fa5.htm#Appendix_A_32" aria-label="Product behavior note 32">&lt;32&gt;</a> The value
of the <b>heightStart</b> field MUST be the following value.</p>

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
  <p>0x04</p>
  </td>
  <td>
  <p>ImageDataProperties.InlineSharedImageDataProperties</p>
  <p>ImageDataProperties.NonSharedImageDataProperties</p>
  </td>
 </tr>
</table>
</dd></dl>

<p><b>heightValue (4 bytes): </b>A signed integer that
specifies the height of an image in pixels. If this property is present, the <a href="c8b60e59-5d3a-4f95-9e2e-fd26420a95e0.htm">Width</a>, <a href="22e8bc7e-11b3-45d7-9a06-fe19d35b73f2.htm">HorizontalResolution</a>, <a href="352ea4d4-5cf3-418b-9211-51ff3f3c0d62.htm">VerticalResolution</a>, and <a href="2430b5fb-8784-4723-b508-cf5996da7c9f.htm">RawFormat</a> properties MUST
be present in the same <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.htm#gt_8502cabb-8fac-401a-93da-3ca2ad4ddf75">parent
record</a>.<a id="Appendix_A_Target_33"></a><a href="1d022514-2a2f-41df-b2f8-36f19e474fa5.htm#Appendix_A_33" aria-label="Product behavior note 33">&lt;33&gt;</a></p>


                </div>
            </div>
        </div>
    </body>
</html>