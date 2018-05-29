<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.81.1 GroupExpressions.GroupExpression</title>
        <xml>
            <mshelp:toctitle title="2.81.1 GroupExpressions.GroupExpression"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: GroupExpressions.GroupExpression"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ce9ab038-c7b6-4ac1-ba9e-faa3a2657eb7"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ce9ab038-c7b6-4ac1-ba9e-faa3a2657eb7"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: GroupExpressions.GroupExpression" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.81.1 GroupExpressions.GroupExpression</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>GroupExpressions.GroupExpression</b> element
specifies an expression by which to group data. This element MUST be specified
at least once and can be specified more than once. The value of this element
MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.1) or an expression that evaluates to a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_a3af3eaf-64b7-499b-a95f-193cd4c27812">Variant</a>. </p>

<p>The value of the <b>GroupExpressions.GroupExpression</b>
element MUST NOT include any <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_1d75df79-dbed-4ab5-8650-588c4e94ba3b">aggregate
functions</a> other than the <a href="5246ac2c-9de7-42a2-9b5a-73484f9fe73b.md">RowNumber</a>
aggregate function. If the RowNumber aggregate function is used, it MUST
reference the immediately containing scope.</p>

<p>Following is the parent element of the <b>GroupExpressions.GroupExpression</b>
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
  <p><a href="81754d26-7dbd-4449-ac41-629f9a8d0feb.md">GroupExpressions</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>GroupExpressions.GroupExpression</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;GroupExpression&quot; type=&quot;xsd:string&quot; maxOccurs=&quot;unbounded&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>