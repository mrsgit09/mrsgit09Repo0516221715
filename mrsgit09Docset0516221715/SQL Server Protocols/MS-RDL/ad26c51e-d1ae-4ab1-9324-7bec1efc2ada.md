<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.111 Title</title>
        <xml>
            <mshelp:toctitle title="2.111 Title"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Title"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ad26c51e-d1ae-4ab1-9324-7bec1efc2ada"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ad26c51e-d1ae-4ab1-9324-7bec1efc2ada"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Title" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.111 Title</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.md"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.md"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>Title</b> element specifies a title for a <a href="b0ab5524-7eb2-47a7-a4d3-230f5c8c5526.md">Chart</a> or for an <a href="2bfb943e-7cfe-41c1-baa4-5739a99a341b.md">Axis</a>.</p>

<p>The following are the parent and child elements of the <b>Title</b>
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
  <p>Chart</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Axis</p>
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
  <p><a href="3fc9d092-506c-47dd-9ee3-611f7691a122.md">Title.Caption</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="52941fb9-e606-4043-bbc2-84a4f617b0cb.md">Title.Position</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="61c04cc7-1d21-4167-816b-6a001f591cdd.md">Title.Style</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Title</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;TitleType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;Caption&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;Style&quot; type=&quot;StyleType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;Position&quot; minOccurs=&quot;0&quot;&gt;
       &lt;xsd:simpleType&gt;
         &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
           &lt;xsd:enumeration value=&quot;Center&quot; /&gt;
           &lt;xsd:enumeration value=&quot;Near&quot; /&gt;
           &lt;xsd:enumeration value=&quot;Far&quot; /&gt;
         &lt;/xsd:restriction&gt;
       &lt;/xsd:simpleType&gt;
     &lt;/xsd:element&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>