<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.9 Report 2008</title>
        <xml>
            <mshelp:toctitle title="3.9 Report 2008"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: Report 2008"></mshelp:rltitle>
            <mshelp:keyword index="A" term="de5b6f5c-5fe5-4bed-aa25-f64fafbbf8b2"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="de5b6f5c-5fe5-4bed-aa25-f64fafbbf8b2"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: Report 2008" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.9 Report 2008</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>This example specifies the records that are required to
produce a <a href="4be143af-2e99-41c5-894d-01902ed98673.htm">Report</a> by
using RPL 10.3.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Offset</p>
   </th>
   <th>
   <p>Size</p>
   </th>
   <th>
   <p>Structure</p>
   </th>
   <th>
   <p>Value</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0201</p>
  </td>
  <td>
  <p><b>Report</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1</p>
  </td>
  <td>
  <p>000B</p>
  </td>
  <td>
  <p>   STRING<b>- RPLStamp</b></p>
  </td>
  <td>
  <p>RPLIF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0006</p>
  </td>
  <td>
  <p>   <b>Version</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xC</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  majorVersion</b></p>
  </td>
  <td>
  <p>0x0A</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  minorVersion</b></p>
  </td>
  <td>
  <p>0x03</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xE</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>      INT<b>- build</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x12</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>   BYTE<b>- reportStart</b></p>
  </td>
  <td>
  <p>0x00</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0017</p>
  </td>
  <td>
  <p>   <b>ReportProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x13</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  reportPropertiesStart</b></p>
  </td>
  <td>
  <p>0x02</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0015</p>
  </td>
  <td>
  <p>      <b>ItemProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x14</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>reportNameStart</b></p>
  </td>
  <td>
  <p>0x0F</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x15</p>
  </td>
  <td>
  <p>000F</p>
  </td>
  <td>
  <p>         STRING
  - <b>reportNameValue</b></p>
  </td>
  <td>
  <p>Report1</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x24</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>autoRefreshStart</b></p>
  </td>
  <td>
  <p>0x0E</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x25</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>         INT
  - <b>autoRefreshValue</b></p>
  </td>
  <td>
  <p>0x0000001E</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x29</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE <b>-
  delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>01B3</p>
  </td>
  <td>
  <p>   <b>PageContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x2A</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  pageContentStart</b></p>
  </td>
  <td>
  <p>0x13</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>00CB</p>
  </td>
  <td>
  <p>      <b>BodyAreaElement</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x2B</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>columns</b></p>
  </td>
  <td>
  <p>0x14</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>005C</p>
  </td>
  <td>
  <p>         <b>BodyArea</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x2C</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>body</b></p>
  </td>
  <td>
  <p>0x06</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0016</p>
  </td>
  <td>
  <p>            <b>ElementProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x2D</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>elementPropertiesStart</b></p>
  </td>
  <td>
  <p>0x0F</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0014</p>
  </td>
  <td>
  <p>               <b>SharedElementProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x2E</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>shared</b></p>
  </td>
  <td>
  <p>0x00</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0012</p>
  </td>
  <td>
  <p>                  <b>ItemProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x2F</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                     BYTE
  - <b>idStart</b></p>
  </td>
  <td>
  <p>0x01</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x30</p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>                     STRING
  - <b>idValue</b></p>
  </td>
  <td>
  <p>BodyArea</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x41</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x42</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>            <b>ReportItems</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x43</p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>               <b>Image</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>002A</p>
  </td>
  <td>
  <p>            <b>Measurements</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x54</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>measurementsStart</b></p>
  </td>
  <td>
  <p>0x10</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x55</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x000000000000002C</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x5D</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               INT<b>-
  count</b></p>
  </td>
  <td>
  <p>0x00000001</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>001D</p>
  </td>
  <td>
  <p>               <b>measurementsContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x61</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x65</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x69</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0x00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x6D</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x00003243</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x71</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x75</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x76</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>                  INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x000000000000004A</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>000A</p>
  </td>
  <td>
  <p>               <b>ReportElementEnd</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x7E</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>elementEnd</b></p>
  </td>
  <td>
  <p>0xFE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x7F</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>                  INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x0000000000000054</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x87</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>002A</p>
  </td>
  <td>
  <p>            <b>Measurements</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x88</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>measurementsStart</b></p>
  </td>
  <td>
  <p>0x10</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x89</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x000000000000002B</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x91</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               INT<b>-
  count</b></p>
  </td>
  <td>
  <p>0x00000001</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>001D</p>
  </td>
  <td>
  <p>                <b>measurementsContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x95</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x99</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x0000CC41</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x9D</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0x00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xA1</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x00003243</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xA5</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xA9</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xAA</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>                  INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x000000000000007E</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>000A</p>
  </td>
  <td>
  <p>            <b>ReportElementEnd</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xB2</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>elementEnd</b></p>
  </td>
  <td>
  <p>0xFE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xB3</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x0000000000000088</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xBB</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>00B3</p>
  </td>
  <td>
  <p>      <b>Page</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xBC</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>pageStart</b></p>
  </td>
  <td>
  <p>0x01</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0019</p>
  </td>
  <td>
  <p>         <b>PageProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xBD</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>pagePropertiesStart</b></p>
  </td>
  <td>
  <p>0x03</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0017</p>
  </td>
  <td>
  <p>            <b>ItemProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xBE</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>idStart</b></p>
  </td>
  <td>
  <p>0x01</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xBF</p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>               STRING
  - <b>idValue</b></p>
  </td>
  <td>
  <p>PageID01</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD0</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>columnsStart</b></p>
  </td>
  <td>
  <p>0x17</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD1</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               INT
  - <b>columnsValue</b></p>
  </td>
  <td>
  <p>0x00000001</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD5</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  <b>- delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>004C</p>
  </td>
  <td>
  <p>         <b>PageHeaderElement</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD6</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>pageHeader</b></p>
  </td>
  <td>
  <p>0x04</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0006</p>
  </td>
  <td>
  <p>            <b>ElementProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD7</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>elementPropertiesStart</b></p>
  </td>
  <td>
  <p>0x0F</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               <b>SharedElementProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD8</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>shared</b></p>
  </td>
  <td>
  <p>0x00</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0002</p>
  </td>
  <td>
  <p>                  <b>ItemProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xD9</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                     BYTE
  - <b>printOnFirstPageStart</b></p>
  </td>
  <td>
  <p>0x2C</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xDA</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                     BYTE
  - <b>printOnFirstPageValue</b></p>
  </td>
  <td>
  <p>0x01</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xDB</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xDC</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>            <b>ReportItems</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xDD</p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>               <b>Line</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>002A</p>
  </td>
  <td>
  <p>            <b>Measurements</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xEE</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>measurementsStart</b></p>
  </td>
  <td>
  <p>0x10</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xEF</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x00000000000000D6</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xF7</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               INT<b>-
  count</b></p>
  </td>
  <td>
  <p>0x00000001</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>001D</p>
  </td>
  <td>
  <p>               <b>measurementsContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xFB</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0xFF</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x103</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0x00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x107</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x0000CC42</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x10B</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x10F</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x110</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>                  INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x00000000000000E4</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>000A</p>
  </td>
  <td>
  <p>            <b>ReportElementEnd</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x118</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>elementEnd</b></p>
  </td>
  <td>
  <p>0xFE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x119</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x00000000000000EE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x121</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>004C</p>
  </td>
  <td>
  <p>         <b>PageFooterElement</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x122</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>pageFooter</b></p>
  </td>
  <td>
  <p>0x05</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0006</p>
  </td>
  <td>
  <p>            <b>ElementProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x123</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>elementPropertiesStart</b></p>
  </td>
  <td>
  <p>0x0F</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               <b>SharedElementProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x124</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>shared</b></p>
  </td>
  <td>
  <p>0x00</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0002</p>
  </td>
  <td>
  <p>                  <b>ItemProperties</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x125</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                     BYTE
  - <b>printOnFirstPageStart</b></p>
  </td>
  <td>
  <p>0x2C</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x126</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                     BYTE
  - <b>printOnFirstPageValue</b></p>
  </td>
  <td>
  <p>0x00</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x127</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x128</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>            <b>ReportItems</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x129</p>
  </td>
  <td>
  <p>0011</p>
  </td>
  <td>
  <p>               <b>Line</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>002A</p>
  </td>
  <td>
  <p>            <b>Measurements</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x13A</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>measurementsStart</b></p>
  </td>
  <td>
  <p>0x10</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x13B</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x000000000000122</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x143</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>               INT<b>-
  count</b></p>
  </td>
  <td>
  <p>0x00000001</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>001D</p>
  </td>
  <td>
  <p>               <b>measurementsContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x147</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x14B</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x14F</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0X00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x153</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x0000CC41</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x157</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>                  INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x15B</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>                  BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x15C</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>                  INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x0000000000000130</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>000A</p>
  </td>
  <td>
  <p>            <b>ReportElementEnd</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x164</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>elementEnd</b></p>
  </td>
  <td>
  <p>0xFE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x165</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>               INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x000000000000013A</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x16D</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>               BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x16E</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0064</p>
  </td>
  <td>
  <p>      <b>Measurements</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x16F</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>measurementsStart</b></p>
  </td>
  <td>
  <p>0x10</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x170</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>         INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x000000000000002A</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x178</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>         INT<b>-
  count</b></p>
  </td>
  <td>
  <p>0x00000003</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0057</p>
  </td>
  <td>
  <p>         <b>measurementsContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x17C</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x180</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x0000CC41</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x184</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0x00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x188</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x00003243</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x18C</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x190</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x191</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>            INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x00000000000000B2</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x199</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x19D</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1A1</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0x00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1A5</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x0000CC41</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1A9</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1AD</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1AE</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>            INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x0000000000000118</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1B6</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>left</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1BA</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>top</b></p>
  </td>
  <td>
  <p>0x00804B43</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1BE</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>width</b></p>
  </td>
  <td>
  <p>0x00001843</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1C2</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            FLOAT
  - <b>height</b></p>
  </td>
  <td>
  <p>0x0000CC41</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1C6</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>            INT
  - <b>zIndex</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1CA</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>            BYTE
  - <b>state</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitTop</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitBottom</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitLeft</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>omitRight</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>hasToggle</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>toggleCollapse</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>1 bit</p>
  </td>
  <td>
  <p>                     BIT
  - <b>reserved</b></p>
  </td>
  <td>
  <p>0x0</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1CB</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>            INT
  - <b>reportElementEndOffset</b></p>
  </td>
  <td>
  <p>0x0000000000000164</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>000A</p>
  </td>
  <td>
  <p>      <b>ReportElementEnd</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1D3</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>elementEnd</b></p>
  </td>
  <td>
  <p>0xFE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1D4</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>         INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x000000000000016F</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1DC</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>         BYTE
  - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0015</p>
  </td>
  <td>
  <p>   <b>OffSetsArrayElement</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1DD</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  offsetsArrayElementStart</b></p>
  </td>
  <td>
  <p>0x12</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1DE</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>      INT<b>- offset</b></p>
  </td>
  <td>
  <p>0x0000000000000012</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1E6</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>      INT<b>- count</b></p>
  </td>
  <td>
  <p>0x00000001</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>      <b>OffsetsPageContent</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1EA</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>         INT<b>-
  offset</b></p>
  </td>
  <td>
  <p>0x00000000000001D3</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>000A</p>
  </td>
  <td>
  <p>   <b>ReportElementEnd</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1F2</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE - <b>elementEnd</b></p>
  </td>
  <td>
  <p>0xFE</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1F3</p>
  </td>
  <td>
  <p>0008</p>
  </td>
  <td>
  <p>      INT<b>- offset</b></p>
  </td>
  <td>
  <p>0x00000000000001DD</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1FB</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE - <b>delimiter</b></p>
  </td>
  <td>
  <p>0xFF</p>
  </td>
 </tr>
 <tr>
  <td>
  <p> </p>
  </td>
  <td>
  <p>0006</p>
  </td>
  <td>
  <p>   <b>Version</b></p>
  </td>
  <td>
  <p> </p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1FC</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  majorVersion</b></p>
  </td>
  <td>
  <p>0x0A</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1FD</p>
  </td>
  <td>
  <p>0001</p>
  </td>
  <td>
  <p>      BYTE<b>-
  minorVersion</b></p>
  </td>
  <td>
  <p>0x03</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>0x1FE</p>
  </td>
  <td>
  <p>0004</p>
  </td>
  <td>
  <p>      INT<b>- build</b></p>
  </td>
  <td>
  <p>0x00000000</p>
  </td>
 </tr>
</table>

<p><b>Report:</b> A Report record specifies the contents
of the report.</p>

<p><b>RPLStamp:</b> The &quot;RPLIF&quot; value
specifies the value for the stamp.</p>

<p><b>Version:</b> A <a href="1478a189-40e0-412a-baf0-caa8b934ca72.htm"><span>Version</span></a> structure specifies the RPL version.</p>

<p><b>majorVersion:</b> 0x0A specifies that the major
version is 10.</p>

<p><b>minorVersion:</b> 0x03 specifies that the minor
version is 3.</p>

<p><b>build:</b> 0x00000000 specifies that the build is
0.</p>

<p><b>reportStart:</b> 0x00 specifies the start token of
the Report record.</p>

<p><b>ReportProperties:</b> A <a href="a9b28610-5438-470d-84bb-0608d07ddc46.htm"><span>ReportProperties</span></a> record specifies properties of the report.</p>

<p><b>reportPropertiesStart:</b> 0x02 specifies the
start token of the ReportProperties record.</p>

<p><b>ItemProperties:</b> An array of item properties
for the Report record.</p>

<p><b>reportNameStart:</b> 0x0F specifies the start
token of the <a href="04f243a8-affa-43cc-9232-ca7254222200.htm"><span>ReportName</span></a> property.</p>

<p><b>reportNameValue:</b> Report1 specifies the name of
the report.</p>

<p><b>autoRefreshStart:</b> 0x0E specifies the start
token of the <a href="d82719c4-59d8-43fd-9de8-89e91e6cf2a0.htm"><span>AutoRefresh</span></a> property.</p>

<p><b>autoRefreshValue:</b> 0x0000001E specifies that
the automatic refresh interval is 30 seconds.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the
ReportProperties record.</p>

<p><b>PageContent:</b> A <a href="031cb41d-d136-43e5-8d0c-bf1fe123f806.htm">PageContent</a>
(RPL 10.3) record specifies the pages of a report.</p>

<p><b>pageContentStart:</b> 0x13 specifies the start
token of the <b>PageContent</b> structure.</p>

<p><b>BodyAreaElement:</b> A <a href="8528a8c1-b350-43a8-b924-28e8113b63c9.htm">BodyAreaElement</a>
(RPL 10.3) record specifies an area of the body of <b>PageContent</b>.</p>

<p><b>Columns:</b> 0x14 specifies the start token of the
<b>BodyAreaElement</b> record.</p>

<p><b>BodyArea:</b> A <a href="fd0b6a17-7759-4674-aa84-bec51908f314.htm">BodyElement</a> record
specifies the content of the main area of <b>BodyAreaElement</b>.</p>

<p><b>body:</b> 0x06 specifies the start token of the <b>BodyArea</b>
record.</p>

<p><b>ElementProperties:</b> An <a href="d7f6cef2-01c6-4562-a4a0-5f205d79963e.htm">ElementProperties</a> record
that specifies the properties for the <b>BodyArea</b> record.</p>

<p><b>elementPropertiesStart:</b> 0x0F specifies the
start token of the <b>ElementProperties</b> record.</p>

<p><b>SharedElementProperties:</b> A <a href="9496b6e7-b12b-4fbe-ad27-2cc5e9d61fcd.htm">SharedElementProperties</a>
record that specifies the <a href="23d76278-cee5-45ee-a361-a9d94d6d3300.htm">InlineSharedElementProperties</a>
record of the <b>BodyArea</b> record.</p>

<p><b>shared:</b> 0x00 specifies the start token of the <b>SharedElementProperties</b>
record.</p>

<p><b>ItemProperties:</b> An array of properties for the
<b>BodyAreaElement</b> record.</p>

<p><b>idStart:</b> 0x01 specifies the start token of the
<a href="cefdcebd-7703-4ba3-a8f1-ba3681283bf7.htm">ID</a> property.</p>

<p><b>idValue:</b> <i>BodyArea</i> specifies <b>ID</b>
for the <b>BodyArea</b> record.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>SharedElementProperties</b>
record.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ElementProperties</b>
record.</p>

<p><b>ReportItems:</b> A <a href="422387f7-880f-4d86-9e88-2a5d2e8f191e.htm">ReportItem</a> record
specifies items in the report.</p>

<p><b>Image:</b> An <a href="b6e7b187-4160-4ce2-940e-6198a7416863.htm">Image</a> record specifies an <b>Image</b>
report item in the <b>BodyArea</b> record. See the <b>Image</b> example
(section <a href="d9153136-89b4-4071-8d0c-613e860be560.htm">3.2</a>) for
additional details.</p>

<p><b>Measurements:</b> A <a href="5c5210d9-a82b-4040-8e79-800e2ee51b52.htm">Measurements</a> record
specifies the measurements of an <b>Image</b> report item.</p>

<p><b>measurementsStart:</b> 0x10 specifies the start
token of the <b>Measurements</b> record.</p>

<p><b>offset:</b> 0x000000000000002C specifies the
position of the body token in the RPL stream.</p>

<p><b>count:</b> 0x00000001 specifies that there is one
measurement record.</p>

<p><b>MeasurementsContent:</b> A <b>MeasurementsContent</b>
record specifies an array of measurements.</p>

<p><b>left:</b> 0x00000000 specifies that the image is
placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x00000000 specifies that the image is
placed 0 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the image is
152 millimeters wide.</p>

<p><b>height:</b> 0x00003243 specifies that the image is
178 millimeters tall.</p>

<p><b>zIndex:</b> 0x00000000 specifies that the image is
drawn first.</p>

<p><b>State:</b> A <a href="3025d1fb-b89c-42ce-b786-7256e321a9e2.htm">State</a> property specifies
the state information for the <b>Measurement</b> record of the report item.</p>

<p><b>A:</b> 0x0 specifies that the top border is not
omitted.</p>

<p><b>B:</b> 0x0 specifies that the bottom border is not
omitted.</p>

<p><b>C:</b> 0x0 specifies that the left border is not
omitted.</p>

<p><b>D:</b> 0x0 specifies that the right border is not
omitted.</p>

<p><b>E:</b> 0x0 specifies that the report item does not
toggle visibility.</p>

<p><b>F:</b> 0x0 specifies that the report item is not
set to collapse.</p>

<p><b>Reserved:</b> 0x0 specifies that the bit is to be
set to 0.</p>

<p><b>Reserved:</b> 0x0 specifies that the bit is to be
set to 0.</p>

<p><b>reportElementEndOffset:</b> 0x000000000000004A
specifies the position of the <b>ReportElementEnd</b> record for the <b>Image</b>
report item structure in the RPL stream.</p>

<p><b>ReportElementEnd:</b> A <a href="75f1a870-2f17-4806-b286-e67c7239e103.htm">ReportElementEnd</a> record
specifies the end of the <b>BodyArea</b> record.</p>

<p><b>elementEnd:</b> 0xFE specifies the start token of
the <b>ReportElementEnd</b> record.</p>

<p><b>offset:</b> 0x0000000000000054 specifies the
position of the <b>measurementsStart</b> token for the <b>BodyArea</b> record
in the RPL stream.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ReportElementEnd</b>
record.</p>

<p><b>Measurements:</b> A <b>Measurements</b> record
specifies the measurements of the body area.</p>

<p><b>measurementsStart:</b> 0x10 specifies the start
token of the <b>Measurements</b> record.</p>

<p><b>offset:</b> 0x000000000000002B specifies the
position of the columns token in the RPL stream.</p>

<p><b>count:</b> 0x00000001 specifies that there is one
measurement record.</p>

<p><b>MeasurementsContent:</b> A <b>MeasurementsContent</b>
structure specifies an array of measurements.</p>

<p><b>left:</b> 0x00000000 specifies that the body area
is placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x0000CC41 specifies that the body area
is placed 25.5 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the body area
is 152 millimeters wide.</p>

<p><b>height:</b> 0x00003243 specifies that the body
area is 178 millimeters tall.</p>

<p><b>zIndex:</b> 0x00000000 specifies that the body
area is drawn first.</p>

<p><b>State:</b> A <b>State</b> property specifies the
state information for the <a href="793e2994-8d9c-4c17-b9a6-7baca8d2d035.htm">Measurement</a>
record of the report item.</p>

<p><b>reportElementEndOffset:</b> 0x000000000000007E
specifies the position of the <b>ReportElementEnd</b> record for the <b>BodyElement</b>
structure in the RPL stream.</p>

<p><b>ReportElementEnd:</b> A <b>ReportElementEnd</b>
record specifies the end of the <b>BodyAreaElement</b> record.</p>

<p><b>elementEnd:</b> 0xFE specifies the start token of
the <b>ReportElementEnd</b> record.</p>

<p><b>offset:</b> 0x0000000000000088 specifies the
position of the <b>measurementsStart</b> token for the <b>BodyAreaElement</b>
record in the RPL stream.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ReportElementEnd</b>
record.</p>

<p><b>Page:</b> A <a href="7675024f-e8f7-4bc1-a889-5ca00ffd8782.htm">Page</a> record specifies a <b>Page</b>
record in <a href="aa2a61ad-6000-40f6-8872-d79f21601b5b.htm">PageContent</a>.</p>

<p><b>pageStart:</b> 0x01 specifies the start token of
the <b>Page</b> record.</p>

<p><b>PageProperties:</b> A <a href="0b56e16b-0d77-4cad-83a4-1ba0c046a35c.htm">PageProperties</a> record
specifies the properties of a page.</p>

<p><b>pagePropertiesStart:</b> 0x03 specifies the start
token of the <b>PageProperties</b> record.</p>

<p><b>ItemProperties:</b> An array of properties for the
<b>Page</b> record.</p>

<p><b>idStart:</b> 0x01 specifies the start token of the
<b>ID</b> property.</p>

<p><b>idValue:</b> <i>PageID01</i> specifies the
identifier for the page.</p>

<p><b>columnsStart:</b> 0x17 specifies the start token
of the <b>ColumnCount</b> property.</p>

<p><b>columnsValue:</b> 0x00000001 specifies that there
is one column in this page.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>PageProperties</b>
record.</p>

<p><b>PageHeaderElement:</b> A <a href="42322dd8-21a8-4c45-9567-393dfa424736.htm">PageHeaderElement</a> record
specifies the header of a page.</p>

<p><b>pageHeader:</b> 0x04 specifies the start token of
the <b>PageHeaderElement</b> record.</p>

<p><b>ElementProperties:</b> An <b>ElementProperties</b>
record specifies the properties for the <b>PageHeaderElement</b> record.</p>

<p><b>elementPropertiesStart:</b> 0x0F specifies the
start token of the <b>ElementProperties</b> record.</p>

<p><b>SharedElementProperties:</b> A <b>SharedElementProperties</b>
record that specifies the shared properties of a <b>pageHeader</b> record.</p>

<p><b>shared:</b> 0x00 specifies the start token of the <b>SharedElementProperties</b>
record.</p>

<p><b>ItemProperties:</b> An array of properties for the
<b>PageHeaderElement</b> record.</p>

<p><b>printOnFirstPageStart:</b> 0x2C specifies the
start token of the <b>PrintOnFirstPage</b> property.</p>

<p><b>printOnFirstPageValue:</b> 0x01 specifies a true
value, which indicates that the page header will print on the first page.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>SharedElementProperties</b>
record.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ElementProperties</b>
record.</p>

<p><b>ReportItems:</b> A ReportItem record that
specifies the items in the report.</p>

<p><b>Line: </b>A <a href="d3902de8-408b-496c-b3a5-554bf393a225.htm">Line</a> record specifies a <b>Line</b>
report item in the <b>PageHeader</b> record. See the <b>Line</b> example
(section <a href="e64e09d2-e36e-45ac-90e9-e9b5b406ec65.htm">3.1</a>) for
additional details.</p>

<p><b>Measurements:</b> A <b>Measurements</b> record
specifies the measurements of the report items.</p>

<p><b>measurementsStart:</b> 0x10 specifies the start
token of the <b>Measurements</b> record.</p>

<p><b>offset:</b> 0x00000000000000D6 specifies the
position of the <b>pageHeader</b> token in the RPL stream.</p>

<p><b>count:</b> 0x00000001 specifies that there is one <b>Measurement</b>
record.</p>

<p><b>MeasurementsContent:</b> A <b>MeasurementsContent</b>
record specifies an array of <b>Measurement</b> records.</p>

<p><b>left:</b> 0x00000000 specifies that the line is
placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x00000000 specifies that the line is
placed 0 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the line is
152 millimeters wide.</p>

<p><b>height:</b> 0x0000CC41 specifies that the line is
25.5 millimeters tall.</p>

<p><b>zIndex:</b> 0x00000000 specifies that the line is
drawn first.</p>

<p><b>State:</b> A <b>State</b> property specifies the
state information for the Measurement record of the report item.</p>

<p><b>reportElementEndOffset:</b> 0x00000000000000E4
specifies the position of the <b>ReportElementEnd</b> record of the <b>Line</b>
report item in the <b>PageHeaderElement</b> record in the RPL stream.</p>

<p><b>ReportElementEnd:</b> A <b>ReportElementEnd</b>
record specifies the end of the <b>PageHeaderElement</b> record.</p>

<p><b>elementEnd:</b> 0xFE specifies the start token of
the <b>ReportElementEnd</b> record.</p>

<p><b>offset:</b> 0x00000000000000EE specifies the
position of the <b>measurementsStart</b> token for the <b>PageHeaderElement</b>
record in the RPL stream.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ReportElementEnd</b>
record.</p>

<p><b>PageFooterElement:</b> A <a href="c6b17d7f-d30f-475d-9839-ff97d9d7d69a.htm">PageFooterElement</a> record
specifies the footer of a page.</p>

<p><b>pageFooter:</b> 0x05 specifies the start token of
the <b>PageFooterElement</b> record.</p>

<p><b>ElementProperties:</b> An ElementProperties record
specifies the properties for the <b>PageFooterElement</b> record.</p>

<p><b>elementPropertiesStart:</b> 0x0F specifies the
start token of the <b>ElementProperties</b> record.</p>

<p><b>SharedElementProperties:</b> A <b>SharedElementProperties</b>
record that specifies the shared properties of a <b>PageFooter</b> record.</p>

<p><b>shared:</b> 0x00 specifies the start token of the <b>SharedElementProperties</b>
record.</p>

<p><b>ItemProperties:</b> An array of properties for the
<b>PageFooterElement</b> record.</p>

<p><b>printOnFirstPageStart:</b> 0x2C specifies the
start token of the <b>PrintOnFirstPage</b> property.</p>

<p><b>printOnFirstPageValue:</b> 0x00 specifies a false
value, which indicates that the page footer will not print on the first page.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>SharedElementProperties</b>
record.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ElementProperties</b>
record.</p>

<p><b>ReportItems:</b> A <b>ReportItem</b> record
specifies items in the report.</p>

<p><b>Line:</b> A <b>Line</b> record specifies a <b>Line</b>
report item in the <b>PageFooter</b> record. See the <b>Line</b> example for
additional details.</p>

<p><b>Measurements:</b> A <b>Measurements</b> record
specifies the measurements of the report items.</p>

<p><b>measurementsStart:</b> 0x10 specifies the start
token of the <b>Measurements</b> structure.</p>

<p><b>offset:</b> 0x0000000000000122 specifies the
position of the <b>pageFooter</b> token in the RPL stream.</p>

<p><b>count:</b> 0x00000001 specifies that there is one <b>Measurement</b>
record.</p>

<p><b>MeasurementsContent:</b> A <b>MeasurementsContent</b>
record specifies an array of <b>Measurement</b> records.</p>

<p><b>left:</b> 0x00000000 specifies that the line is
placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x00000000 specifies that the line is
placed 0 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the line is
152 millimeters wide.</p>

<p><b>height:</b> 0x0000CC41 specifies that the line is
25.5 millimeters tall.</p>

<p><b>zIndex:</b> 0x00000000 specifies that the line is
drawn first.</p>

<p><b>State:</b> A <b>State</b> property specifies the
state information for the <b>Measurement</b> record of the report item.</p>

<p><b>reportElementEndOffset:</b> 0x0000000000000130
specifies the position of the <b>ReportElementEnd</b> record of the <b>Line</b>
report item in the <b>PageFooterElement</b> record in the RPL stream.</p>

<p><b>ReportElementEnd:</b> A <b>ReportElementEnd</b>
record specifies the end of the <b>PageFooterElement</b> record.</p>

<p><b>elementEnd:</b> 0xFE specifies the start token of
the <b>ReportElementEnd</b> record.</p>

<p><b>offset:</b> 0x000000000000013A specifies the
position of the <b>measurementsStart</b> token for the <b>PageFooterElement</b>
record in the RPL stream.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ReportElementEnd</b>
record.</p>

<p><b>Measurements:</b> A <b>Measurements</b> record
specifies the measurements of the <b>PageContent (RPL 10.3)</b> record.</p>

<p><b>measurementsStart:</b> 0x10 specifies the start
token of the <b>Measurements</b> record.</p>

<p><b>offset:</b> 0x000000000000002A specifies the
position of the <b>pageContentStart</b> token in the RPL stream.</p>

<p><b>count:</b> 0x00000003 specifies that there are
three <b>Measurement</b> records.</p>

<p><b>MeasurementsContent:</b> A <b>MeasurementsContent</b>
record specifies an array of <b>Measurement</b> records.</p>

<p><b>left:</b> 0x00000000 specifies that the body area
is placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x0000CC41 specifies that the body area
is placed 25.5 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the body area
is 152 millimeters wide.</p>

<p><b>height:</b> 0x00003243 specifies that the body
area is 178 millimeters tall.</p>

<p><b>zIndex:</b> 0x00000000 specifies that the body
area is drawn first.</p>

<p><b>State:</b> A <b>State</b> property specifies the
state information for the <b>Measurement</b> record of the report item.</p>

<p><b>reportElementEndOffset:</b> 0x000000000000007E
specifies the position of the <b>ReportElementEnd</b> record for the <b>Body</b>
record in the RPL stream.</p>

<p><b>left:</b> 0x00000000 specifies that the page
header is placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x00000000 specifies that the page header
is placed 0 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the page
header is 152 millimeters wide.</p>

<p><b>height:</b> 0x0000CC41 specifies that the page
header is 25.5 millimeters all.</p>

<p><b>zIndex:</b> 0x00000001 specifies that the page
header is drawn second.</p>

<p><b>State:</b> A <b>State</b> property specifies the
state information for the <b>Measurement</b> record of the page header.</p>

<p><b>reportElementEndOffset:</b> 0x0000000000000118
specifies the position of the <b>ReportElementEnd</b> record for the <b>PageHeader</b>
record in the RPL stream.</p>

<p><b>left:</b> 0x00000000 specifies that the page
footer is placed 0 millimeters to the left of the parent.</p>

<p><b>top:</b> 0x00804B43 specifies that the page footer
is placed 203.5 millimeters below the parent. </p>

<p><b>width:</b> 0x00001843 specifies that the page
footer is 152 millimeters wide.</p>

<p><b>height:</b> 0x0000CC41 specifies that the page
footer is 25.5 millimeters tall.</p>

<p><b>zIndex:</b> 0x00000002 specifies that the page
footer is drawn third.</p>

<p><b>State:</b> A <b>State</b> property specifies the
state information for the <b>Measurement</b> record of the page footer.</p>

<p><b>reportElementEndOffset:</b> 0x0000000000000164
specifies the position of the <b>ReportElementEnd</b> record for the <b>PageFooter</b>
record in the RPL stream.</p>

<p><b>ReportElementEnd</b>: A <b>ReportElementEnd</b>
record specifies the end of <b>PageContent</b>.</p>

<p><b>elementEnd:</b> 0xFE specifies the start token of
the <b>ReportElementEnd</b> record.</p>

<p><b>offset:</b> 0x000000000000016F specifies the
position of the <b>measurementsStart</b> token for the <b>PageContent</b>
record in the RPL stream.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ReportElementEnd</b>
record.</p>

<p><b>OffsetsArrayElement:</b> An <a href="c79d94ee-588b-4c7a-b3ba-4dc5dc820ae7.htm">OffsetsArrayElement</a> record
specifies the <b>offset</b> for each page.</p>

<p><b>offsetsArrayElementStart:</b> 0x12 specifies the
start token of the <b>OffsetsArrayElement</b> structure.</p>

<p><b>offset:</b> 0x0000000000000012 specifies the
position of the <b>reportStart</b> token in the RPL stream.</p>

<p><b>count:</b> 0x00000001 specifies that there is one <b>PageContent</b>
record.</p>

<p><b>OffsetsPageContent:</b> An <b>OffsetsPageConent</b>
record specifies an array with offsets to each <b>reportElementEnd</b> field of
a <b>PageContent</b> record in the RPL stream.</p>

<p><b>offset:</b> 0x00000000000001D3 specifies the
position of the <b>ReportElementEnd</b> record for the <b>PageContent</b>
record in the RPL stream.</p>

<p><b>ReportElementEnd:</b> A <b>ReportElementEnd</b>
record specifies the end of the Report.</p>

<p><b>elementEnd:</b> 0xFE specifies the start token of
the <b>ReportElementEnd</b> record.</p>

<p><b>offset:</b> 0x00000000000001DD specifies the
position of the <b>offsetsArrayElementStart</b> token in the RPL stream.</p>

<p><b>delimiter:</b> 0xFF specifies the end of the <b>ReportElementEnd</b>
record.</p>

<p><b>Version:</b> A Version structure specifies the RPL
version.</p>

<p><b>majorVersion:</b> 0x0A specifies that the major
version is 10.</p>

<p><b>minorVersion:</b> 0x03 specifies that the minor
version is 3.</p>

<p><b>build:</b> 0x00000000 specifies that the build is
0.</p>


                </div>
            </div>
        </div>
    </body>
</html>