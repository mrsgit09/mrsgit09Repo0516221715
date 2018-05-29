<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.5.21 HierarchyType</title>
        <xml>
            <mshelp:toctitle title="2.2.5.21 HierarchyType"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: HierarchyType"></mshelp:rltitle>
            <mshelp:keyword index="A" term="28dfbbfa-0df5-4d63-80fa-f44cec7f382d"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="28dfbbfa-0df5-4d63-80fa-f44cec7f382d"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: HierarchyType" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.5.21 HierarchyType</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>HierarchyType</b> simple type specifies the type of
hierarchy to which the entity or entities belong.</p>

<p>The following is the XML schema definition of the <b>HierarchyType</b>
simple type.</p>

<dl>
<dd>
<div><pre> &lt;xs:simpleType name=&quot;HierarchyType&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:restriction base=&quot;xs:string&quot;&gt;
     &lt;xs:enumeration value=&quot;Explicit&quot; /&gt;
     &lt;xs:enumeration value=&quot;Derived&quot; /&gt;
     &lt;xs:enumeration value=&quot;Collection&quot; /&gt;
     &lt;xs:enumeration value=&quot;All&quot; /&gt;
   &lt;/xs:restriction&gt;
 &lt;/xs:simpleType&gt;
</pre></div>
</dd></dl>

<p>The values of the enumeration are described in the following
table.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Value</p>
   </th>
   <th>
   <p>Meaning</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>Explicit</p>
  </td>
  <td>
  <p>The relationship type is explicitly defined.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Derived</p>
  </td>
  <td>
  <p>The relationship type is derived from attribute
  values.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>Collection</p>
  </td>
  <td>
  <p>The relationship type is a collection of hierarchy
  types.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>All</p>
  </td>
  <td>
  <p>All hierarchy types are used.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>