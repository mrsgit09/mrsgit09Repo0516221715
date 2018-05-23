<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.110.9 ThreeDProperties.ProjectionMode</title>
        <xml>
            <mshelp:toctitle title="2.110.9 ThreeDProperties.ProjectionMode"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: ThreeDProperties.ProjectionMode"></mshelp:rltitle>
            <mshelp:keyword index="A" term="a3b6d3f4-fabd-4b82-af8d-bb929ccdf8a3"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="a3b6d3f4-fabd-4b82-af8d-bb929ccdf8a3"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: ThreeDProperties.ProjectionMode" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.110.9 ThreeDProperties.ProjectionMode</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.md"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.md"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>ThreeDProperties.ProjectionMode</b> element specifies
the projection mode used for a 3D rendering. This element is optional. If this
element is present, its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) that is one of the following:</p>

<p><b>Perspective</b> (default): Specifies that
perspective projection is used.</p>

<p><b>Ortographic</b>: Specifies that ortographic
projection is used.</p>

<p>If the <b>ThreeDProperties.ProjectionMode</b> element is not
present, its value is interpreted as &quot;Perspective&quot;.</p>

<p>Following is the parent element of the <b>ThreeDProperties.ProjectionMode</b>
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
  <p><a href="2617763c-2b85-4f0d-9e3f-1828abb52b23.md">ThreeDProperties</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>ThreeDProperties.ProjectionMode</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;ProjectionMode&quot; minOccurs=&quot;0&quot;&gt;
   &lt;xsd:simpleType&gt;
     &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
       &lt;xsd:enumeration value=&quot;Perspective&quot; /&gt;
       &lt;xsd:enumeration value=&quot;Orthographic&quot; /&gt;
     &lt;/xsd:restriction&gt;
   &lt;/xsd:simpleType&gt;
 &lt;/xsd:element&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>