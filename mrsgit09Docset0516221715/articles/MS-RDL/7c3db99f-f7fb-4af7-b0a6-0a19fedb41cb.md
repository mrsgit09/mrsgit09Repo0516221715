<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.46 Slider</title>
        <xml>
            <mshelp:toctitle title="2.46 Slider"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Slider"></mshelp:rltitle>
            <mshelp:keyword index="A" term="7c3db99f-f7fb-4af7-b0a6-0a19fedb41cb"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="7c3db99f-f7fb-4af7-b0a6-0a19fedb41cb"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Slider" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.46 Slider</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.htm"><b><i>RDL 2011/01</i></b></a></p>

<p>The <b>Slider</b> element specifies the <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.htm#gt_de562f82-95a1-4b96-a94e-0e6e3c15dd97">slider metadata</a> for band
navigation.</p>

<p>The following are the parent and child elements of the <b>Slider</b>
element.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Parent elements</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="abc2c5cb-891e-4b78-baec-9b692f1f388a.htm">Coverflow</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="7d46e0bb-d38a-4c70-966c-37302e7f3315.htm">Tabstrip</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="acda9c21-394e-4fea-91ec-24e988e9d4f7.htm">PlayAxis</a></p>
  </td>
 </tr>
</table>

<p> </p>

<table>
 <thead>
  <tr>
   <th>
   <p>Child elements</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="e3046f50-3b68-4dcb-83d6-01315282a2fd.htm">Hidden</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="062db763-8882-4662-895c-71fe98d16b14.htm">LabelData</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Slider</b>
element.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;SliderType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;Hidden&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;LabelData&quot; type=&quot;LabelDataType&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>