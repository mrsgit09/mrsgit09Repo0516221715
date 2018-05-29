<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.2.2.3.1 ComAssembly</title>
        <xml>
            <mshelp:toctitle title="2.2.4.2.2.3.1 ComAssembly"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: ComAssembly"></mshelp:rltitle>
            <mshelp:keyword index="A" term="5b37afe9-44cf-46c7-b61a-aefc3e96afe5"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="5b37afe9-44cf-46c7-b61a-aefc3e96afe5"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: ComAssembly" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.2.2.3.1 ComAssembly</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>ComAssembly</b> complex type represents a <a href="8676f5ce-62d4-4244-a326-634bfed4aba4.html#gt_ef2ebebc-1760-407a-9ace-af48f9050e02">Component Object Model (COM)</a>
library.</p>

<p><b>ComAssembly</b> is derived from <a href="8b1309de-224c-4d8c-b5b1-66dd1e85dbe0.html">Assembly</a>.</p>

<p>COM assemblies treat ImpersonationMode=Default as
ImpersonateCurrentUser. COM assemblies do not support impersonation modes other
than ImpersonateCurrentUser.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;ComAssembly&quot;&gt;
     &lt;xsd:complexContent&gt;
       &lt;xsd:extension base=&quot;Assembly&quot;&gt;
         &lt;xsd:sequence&gt;
           &lt;xsd:element name=&quot;Source&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;/&gt;
         &lt;/xsd:sequence&gt;
       &lt;/xsd:extension &gt;
     &lt;/xsd:complexContent&gt;
   &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following table describes the elements that are included
in the XSD schema for <b>ComAssembly</b>. Those elements common to all major
objects are described in section <a href="b38dcecd-e3a9-4c61-bd35-a7a426ca794e.html">2.2.4.2.2.1</a>. Also included
in <b>ComAssembly</b> are all the elements from <b>Assembly</b> as described in
section 2.2.4.2.2.3.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Element</p>
   </th>
   <th>
   <p>Read-only</p>
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
  <p>Source</p>
  </td>
  <td>
  <p> </p>
  </td>
  <td>
  <p>Empty</p>
  </td>
  <td>
  <p>This element MUST contain either a file name or a PROG
  ID (program ID).</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>