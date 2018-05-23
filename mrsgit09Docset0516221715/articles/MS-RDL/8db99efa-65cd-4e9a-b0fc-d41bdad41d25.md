<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.84.3 Grouping.DataCollectionName</title>
        <xml>
            <mshelp:toctitle title="2.84.3 Grouping.DataCollectionName"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Grouping.DataCollectionName"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8db99efa-65cd-4e9a-b0fc-d41bdad41d25"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8db99efa-65cd-4e9a-b0fc-d41bdad41d25"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Grouping.DataCollectionName" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.84.3 Grouping.DataCollectionName</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="a7e2ad00-07c8-4f6d-80ab-3ad55df7b233.html"><b><i>RDL 2003/10</i></b></a><b>
<i>and </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.html"><b><i>RDL 2005/01</i></b></a></p>

<p>The <b>Grouping.DataCollectionName</b> element specifies the
name to use for the data element in a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_9069c206-b9e9-4374-a7ee-50faf5def25b">data rendering</a> that is the
collection of all instances of this <a href="7d574154-eefe-4fc1-8b78-3a18b9350e87.html">Grouping</a>. This element is
optional.</p>

<p>If this element is present, its value MUST be a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.html#gt_cb2ad790-a668-429f-84fa-f3dd67517e9b">CLS-compliant identifier</a> <a href="https://go.microsoft.com/fwlink/?LinkId=147989">[UTR15]</a>. If this
element is not present, its value is interpreted as the string that is the
concatenation of the value of <a href="cb123eb2-2c24-49d1-814c-d08c878f5820.html">Grouping.DataElementName</a>
and the string &quot;_Collection&quot;. If <b>Grouping.DataElementName</b> is
not specified, its default value is used. In this case, the string that is the
concatenation of the value of <a href="4d08883b-d937-4d6e-b0b2-5dec684678ec.html">Grouping.Name</a> and the
string &quot;_Collection&quot; is used as the default value of <b>Grouping.DataCollectionName</b>.</p>

<p>Following is the parent element of the <b>Grouping.DataCollectionName</b>
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
  <p>Grouping</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Grouping.DataCollectionName</b>
element.           </p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;DataCollectionName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>