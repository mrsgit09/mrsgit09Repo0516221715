<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.3.2.1.1.19.1 Source</title>
        <xml>
            <mshelp:toctitle title="3.1.4.3.2.1.1.19.1 Source"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: Source"></mshelp:rltitle>
            <mshelp:keyword index="A" term="34e94cfa-894d-477f-bb72-ab5efff9ccae"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="34e94cfa-894d-477f-bb72-ab5efff9ccae"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: Source" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.3.2.1.1.19.1 Source</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Source</b> type specifies the source for the
Synchronization command.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;Source&quot;&gt;
     &lt;xsd:all&gt;
       &lt;xsd:element name=&quot;Object&quot; type=&quot;ObjectReference&quot; /&gt;
       &lt;xsd:element name=&quot;ConnectionString&quot; type=&quot;xsd:string&quot; /&gt;
     &lt;/xsd:all&gt;
   &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<table>
 <thead>
  <tr>
   <th>
   <p>Element</p>
   </th>
   <th>
   <p>Default value</p>
   </th>
   <th>
   <p>Description</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>Object</p>
  </td>
  <td>
  <p>[Required]</p>
  </td>
  <td>
  <p>An <b>ObjectReference</b> to the database that is the
  source of the synchronization. The <b>ObjectReference</b> type is defined in
  section <a href="26834101-a86b-4365-8e58-d6e4a6ad377d.htm">3.1.4.3.2.1.1.1</a>.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ConnectionString</p>
  </td>
  <td>
  <p>[Required]</p>
  </td>
  <td>
  <p>The connection string to the source server.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>