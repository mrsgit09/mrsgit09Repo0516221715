<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.13.2.1 NeedRefreshCubeReply</title>
        <xml>
            <mshelp:toctitle title="2.2.13.2.1 NeedRefreshCubeReply"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS8]: NeedRefreshCubeReply"></mshelp:rltitle>
            <mshelp:keyword index="A" term="7b3b80a0-bf8a-45fb-bbbe-3bf9f7ae8d74"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="7b3b80a0-bf8a-45fb-bbbe-3bf9f7ae8d74"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS8]: NeedRefreshCubeReply" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.13.2.1 NeedRefreshCubeReply</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>This response data structure specifies the version of the
dimension and the number of members in the dimension.           </p>

<dl>
<dd>
<div><pre> NeedRefreshCubeReply=
 STATUS
 OPEN(182)
 INT32(183) 
 INT32(184)
 REAL64(185) 
 INT32(186) 
 CLOSE
</pre></div>
</dd></dl>

<table>
 <thead>
  <tr>
   <th>
   <p>Value</p>
   </th>
   <th>
   <p>Meaning</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>STATUS</p>
  </td>
  <td>
  <p>RESPONSESTATUS MUST be 8.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Open(182)</p>
  </td>
  <td>
  <p>Indicates the start of the response.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>INT32(183)</p>
  </td>
  <td>
  <p>A value that specifies the dimension version within
  the cube.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>INT32(184)</p>
  </td>
  <td>
  <p>A value that specifies the version of the cube
  structure.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>REAL64(185)</p>
  </td>
  <td>
  <p>A value that specifies the date and timestamp of the
  last change to the cube or dimension.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>INT32(186)</p>
  </td>
  <td>
  <p>A value that specifies the number of dimensions.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Close</p>
  </td>
  <td>
  <p>Indicates the end of the response.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>