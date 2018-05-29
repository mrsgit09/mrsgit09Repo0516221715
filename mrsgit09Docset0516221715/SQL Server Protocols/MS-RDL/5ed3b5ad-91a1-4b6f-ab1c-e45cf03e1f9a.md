<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.270.5 CustomData.Filters</title>
        <xml>
            <mshelp:toctitle title="2.270.5 CustomData.Filters"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: CustomData.Filters"></mshelp:rltitle>
            <mshelp:keyword index="A" term="5ed3b5ad-91a1-4b6f-ab1c-e45cf03e1f9a"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="5ed3b5ad-91a1-4b6f-ab1c-e45cf03e1f9a"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: CustomData.Filters" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.270.5 CustomData.Filters</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="3ebe2912-4958-4832-b391-cad1f5e13338.md"><b><i>RDL 2005/01</i></b></a><b><i>,
</i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>CustomData.Filters</b> element specifies expressions
that are applied as a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_ffbe7b55-8e84-4f41-a18d-fc29191a4cda">filter</a>
to the data for each row of a <a href="6bb7b35c-e517-4444-a96b-9f2ccdd1a642.md">CustomReportItem</a>. This
element is optional and MUST NOT be specified more than once. If this element
is present, it is of type <a href="4075354a-2747-4ce0-ba0f-3e32a950f605.md">Filters</a>.</p>

<p>Following is the parent element of the <b>CustomData.Filters</b>
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
  <p><a href="7c5c39bd-6a38-4d28-805b-63959242c268.md">CustomData</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>CustomData.Filters</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;Filters&quot; type=&quot;FiltersType&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>