<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.5.2.2.1 INT32(530) – SAFETY_OPTIONS</title>
        <xml>
            <mshelp:toctitle title="2.2.5.2.2.1 INT32(530) – SAFETY_OPTIONS"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS8]: INT32(530) – SAFETY_OPTIONS"></mshelp:rltitle>
            <mshelp:keyword index="A" term="f894938b-0a7a-478a-bfeb-b91cbadaaccb"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="f894938b-0a7a-478a-bfeb-b91cbadaaccb"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS8]: INT32(530) – SAFETY_OPTIONS" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.5.2.2.1 INT32(530) – SAFETY_OPTIONS</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>This value defines default safety options of the <a href="c527450b-f5bd-424b-8c98-ba6365288f35.htm#gt_a0c8d97b-322c-4117-8525-37e5f26751e7">cube</a>.</p>

<p><b>Note</b>   For more information, see <a href="https://go.microsoft.com/fwlink/?linkid=864709">[MSDN-SafetyOptions]</a>.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Symbolic name</p>
   </th>
   <th>
   <p>Value</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>DBPROPVAL_MSMD_SAFETY_OPTIONS_DEFAULT</p>
  </td>
  <td>
  <p>0</p>
  </td>
  <td>
  <p>For connections through HTTP or HTTPS, this value is
  the same as DBPROPVAL_MSMD_SAFETY_OPTIONS_ALLOW_SAFE.</p>
  <p>For all other connections, this value is the same as
  DBPROPVAL_MSMD_SAFETY_OPTIONS_ALLOW_ALL.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DBPROPVAL_MSMD_SAFETY_OPTIONS_ALLOW_ALL</p>
  </td>
  <td>
  <p>1</p>
  </td>
  <td>
  <p>This value enables all user-defined function libraries
  without verifying that they are safe for initialization and scripting.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DBPROPVAL_MSMD_SAFETY_OPTIONS_ALLOW_SAFE</p>
  </td>
  <td>
  <p>2</p>
  </td>
  <td>
  <p>This value indicates that all classes for a particular
  user-defined function library are checked to make sure that they are safe for
  initialization and scripting.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DBPROPVAL_MSMD_SAFETY_OPTIONS_ALLOW_NONE</p>
  </td>
  <td>
  <p>3</p>
  </td>
  <td>
  <p>This value prevents user-defined functions from being
  used during the session.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>