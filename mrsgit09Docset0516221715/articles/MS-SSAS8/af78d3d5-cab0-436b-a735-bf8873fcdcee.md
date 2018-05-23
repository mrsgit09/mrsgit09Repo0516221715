<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.10.1.3.5.1 CellFormulas</title>
        <xml>
            <mshelp:toctitle title="2.2.10.1.3.5.1 CellFormulas"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS8]: CellFormulas"></mshelp:rltitle>
            <mshelp:keyword index="A" term="af78d3d5-cab0-436b-a735-bf8873fcdcee"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="af78d3d5-cab0-436b-a735-bf8873fcdcee"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS8]: CellFormulas" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.10.1.3.5.1 CellFormulas</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The syntax is defined as follows:</p>

<dl>
<dd>
<div><pre> CellFormulas = 
 OPEN(503)
   Int32(504)
 *CellFormula
   CLOSE
</pre></div>
</dd></dl>

<table>
 <thead>
  <tr>
   <th>
   <p>Element</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>OPEN(503)</p>
  </td>
  <td>
  <p>A common data structure that indicates the beginning
  of the element.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(504)</p>
  </td>
  <td>
  <p>This value indicates the number of cell formulas.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>*CellFormula</p>
  </td>
  <td>
  <p>Repeat for each entry.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>CLOSE</p>
  </td>
  <td>
  <p>A common data structure that indicates the end of the
  element.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>