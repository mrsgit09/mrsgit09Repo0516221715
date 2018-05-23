<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.10.1.3.5.1.1 CellFormula</title>
        <xml>
            <mshelp:toctitle title="2.2.10.1.3.5.1.1 CellFormula"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS8]: CellFormula"></mshelp:rltitle>
            <mshelp:keyword index="A" term="eabebdba-e7b4-43af-8a77-3a41fafa9e8d"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="eabebdba-e7b4-43af-8a77-3a41fafa9e8d"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS8]: CellFormula" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.10.1.3.5.1.1 CellFormula</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The syntax is defined as follows.           </p>

<dl>
<dd>
<div><pre> CellFormula= 
 String(505)
 String(506)
 Int32(507)
 DATASET(508)
 DATASET(509) 
 SLICE(510)
 Array(529, length) 
 String(511)
 String(512)
 Int32(513)
 Int32(514)
 Int32(515)
 Int32(516) 
 Int32(528) 
 [String(517)]
 [String(518)]
 [UInt16(519)]
 [UInt16(520)]
 [UInt32(521)]
 [UInt32(522)]
 String(523)
 String(524)                      
 String(525)                        
 String(526)                             
 String(527)                     
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
  <p>String(505)</p>
  </td>
  <td>
  <p>This value indicates name of the CELL CALCULATION.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(506)</p>
  </td>
  <td>
  <p>This value provides a description.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(507)</p>
  </td>
  <td>
  <p>This value indicates whether the calculation utilizes
  an internal optimization code pathway.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DATASET(508)</p>
  </td>
  <td>
  <p>Only if INT32(507)=TRUE. The Top space of the
  optimization calculation.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>DATASET(509)</p>
  </td>
  <td>
  <p>Only if INT32(507)=TRUE. The Bottom space of the
  optimization calculation.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>SLICE(510)</p>
  </td>
  <td>
  <p>This value indicates Slicers (number of levels in the
  cube + 1 (<a href="c527450b-f5bd-424b-8c98-ba6365288f35.html#gt_70548cb6-ef0e-4f2a-8e34-7293a9df8998">measure</a>)).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Array(529, length)</p>
  </td>
  <td>
  <p>An array of masks, one for each dimension. The length
  of this array in bytes will be the number of dimensions times the size of an
  INT32 on the hardware.</p>
  <p>Include calculated members. 0x00000001</p>
  <p>Include specified member only,</p>
  <p>no descendants: 0x00000002</p>
  <p>Verify range, leaves only. 0x00000004</p>
  <p>Verify range, non-leaves only. 0x00000008</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(511)</p>
  </td>
  <td>
  <p>This value is <a href="c527450b-f5bd-424b-8c98-ba6365288f35.html#gt_9b631ff5-dc89-45f0-a1c2-db6981e4804f">MDX</a> that represents the
  CONDITON part of the expression.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(512)</p>
  </td>
  <td>
  <p>This value is MDX that represents the calculation part
  of the expression.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(513)</p>
  </td>
  <td>
  <p>This value indicates a <a href="c527450b-f5bd-424b-8c98-ba6365288f35.html#gt_a611caab-b948-463e-ac07-e9a2f30222a9">calculation pass</a>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(514)</p>
  </td>
  <td>
  <p>This value indicates the depth of the calculation
  pass.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(515)</p>
  </td>
  <td>
  <p>This value indicates a <a href="c527450b-f5bd-424b-8c98-ba6365288f35.html#gt_7faee801-7705-424a-8e64-1cd18ab0dfab">solve order</a>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(516)</p>
  </td>
  <td>
  <p>This value indicates a Protocol State Mask</p>
  <p>defined on server: 0x00000001</p>
  <p>Disabled; client will ignore: 0x00000002</p>
  <p>HIDDEN in schema <a href="c527450b-f5bd-424b-8c98-ba6365288f35.html#gt_43e5a26f-e51f-4f1e-9818-e70bcb25de35">rowsets</a>: 0x00000004</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Int32(528)</p>
  </td>
  <td>
  <p>This value indicates a Protocol Attribute Mask</p>
  <p>Has format property (user setting): 0x00000001</p>
  <p>Has font name property: 0x00000002</p>
  <p>Has font size property: 0x00000004</p>
  <p>Has font attribute property: 0x00000008</p>
  <p>Has back color property: 0x00000010</p>
  <p>Has fore color property: 0x00000020</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>[String(517)]</p>
  </td>
  <td>
  <p>Format property value, optional only if the Format
  Attribute Mask is set (INT32(528) has 0x00000001 set).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>[String(518)]</p>
  </td>
  <td>
  <p>FontName property value, optional only if attribute
  mask is set (INT32(528) has 0x00000002 set).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>[UInt16(519)]</p>
  </td>
  <td>
  <p>FontSize property value, optional only if attribute
  mask is set. (INT32(528) has 0x00000004 set).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>[UInt16(520)]</p>
  </td>
  <td>
  <p>FontAttribute property value, optional only if
  attribute mask is set (INT32(528) has 0x00000008 set).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>[UInt32(521)]</p>
  </td>
  <td>
  <p>Background Color property value, optional only if
  attribute mask is set (INT32(528) has 0x00000010 set).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>[UInt32(522)]</p>
  </td>
  <td>
  <p>Foreground Color property value, optional only if
  attribute mask is set (INT32(528) has 0x00000020 set).</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(523)</p>
  </td>
  <td>
  <p>Background color property value.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(524)</p>
  </td>
  <td>
  <p>Foreground color property value.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(525)</p>
  </td>
  <td>
  <p>Font size property value.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(526)</p>
  </td>
  <td>
  <p>Font attribute property value.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>String(527)</p>
  </td>
  <td>
  <p>Font name property value.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>