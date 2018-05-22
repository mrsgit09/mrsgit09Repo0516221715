<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.305 EmbeddedImage</title>
        <xml>
            <mshelp:toctitle title="2.305 EmbeddedImage"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: EmbeddedImage"></mshelp:rltitle>
            <mshelp:keyword index="A" term="6cdb345a-b502-4eee-84fd-de5ccf2a40e7"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="6cdb345a-b502-4eee-84fd-de5ccf2a40e7"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: EmbeddedImage" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.305 EmbeddedImage</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>EmbeddedImage</b> element specifies an image that is
embedded within a <a href="6bbaafec-020b-406c-b4e7-5e4318b616cb.htm">Report</a>.
The <b>EmbeddedImage</b> element MUST be specified at least once within an <a href="d3bd24c7-cf82-4f98-bf94-a6716af81492.htm">EmbeddedImages</a> collection.</p>

<p>The following are the parent elements, attributes, and child
elements of the <b>EmbeddedImage</b> element.</p>

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
  <p>EmbeddedImages</p>
  </td>
 </tr>
</table>

<p> </p>

<table>
 <thead>
  <tr>
   <th>
   <p>Attributes</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="29fb5117-7c56-40df-a83c-0c6a09cc6947.htm">EmbeddedImage.Name</a></p>
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
  <p><a href="39f1bb55-eee9-4eb8-870d-e8b83487b6f4.htm">EmbeddedImage.ImageData</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="83a812fd-0959-410e-ba65-7929435ca6d7.htm">EmbeddedImage.MIMEType</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>EmbeddedImage</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;EmbeddedImageType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;MIMEType&quot; type=&quot;xsd:string&quot; /&gt;
     &lt;xsd:element name=&quot;ImageData&quot; type=&quot;xsd:string&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:attribute name=&quot;Name&quot; type=&quot;xsd:normalizedString&quot; use=&quot;required&quot; /&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
  
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>