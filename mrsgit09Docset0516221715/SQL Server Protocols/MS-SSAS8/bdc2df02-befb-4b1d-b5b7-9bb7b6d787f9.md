<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.10.1.3.2 INT32(397) Unique Name Style Property</title>
        <xml>
            <mshelp:toctitle title="2.2.10.1.3.2 INT32(397) Unique Name Style Property"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS8]: INT32(397) Unique Name Style Property"></mshelp:rltitle>
            <mshelp:keyword index="A" term="bdc2df02-befb-4b1d-b5b7-9bb7b6d787f9"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="bdc2df02-befb-4b1d-b5b7-9bb7b6d787f9"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS8]: INT32(397) Unique Name Style Property" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.10.1.3.2 INT32(397) Unique Name Style Property</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>See <a href="https://go.microsoft.com/fwlink/?linkid=864708">[MSDN-MDXUniqueNameStyle]</a>
for more information.</p>

<p>Use this property to specify the algorithm for generating
unique names according to the values below.</p>

<table>
 <thead>
  <tr>
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
  <p>0</p>
  </td>
  <td>
  <p>Default. For compatibility with earlier versions, this
  is the same as Value 2. The meaning of this default value is subject to
  change in future versions.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>1</p>
  </td>
  <td>
  <p>Key path algorithm: [dim].&amp;[k1].&amp;[k2]</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>2</p>
  </td>
  <td>
  <p>Compatible with version 7.0, name path algorithm:
  [dim].[n1].[n2]</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>3</p>
  </td>
  <td>
  <p>Compatible with SQL Server 2000 Analysis Services. The
  algorithm uses guaranteed unique names, which are stable over time.</p>
  </td>
 </tr>
</table>


                </div>
            </div>
        </div>
    </body>
</html>