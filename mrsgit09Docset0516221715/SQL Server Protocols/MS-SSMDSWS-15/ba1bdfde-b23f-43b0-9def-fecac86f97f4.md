<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.5.41 TransactionType</title>
        <xml>
            <mshelp:toctitle title="2.2.5.41 TransactionType"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: TransactionType"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ba1bdfde-b23f-43b0-9def-fecac86f97f4"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ba1bdfde-b23f-43b0-9def-fecac86f97f4"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: TransactionType" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.5.41 TransactionType</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>TransactionType</b> simple type specifies the type of
member change that is identified in a transaction.</p>

<p>The following is the XML schema definition of the <b>TransactionType</b>
simple type.</p>

<dl>
<dd>
<div><pre> &lt;xs:simpleType name=&quot;TransactionType&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:restriction base=&quot;xs:string&quot;&gt;
     &lt;xs:enumeration value=&quot;NotSpecified&quot; /&gt;
     &lt;xs:enumeration value=&quot;CreateMember&quot; /&gt;
     &lt;xs:enumeration value=&quot;ChangeMemberStatus&quot; /&gt;
     &lt;xs:enumeration value=&quot;SetAttributeValue&quot; /&gt;
     &lt;xs:enumeration value=&quot;MoveMemberToParent&quot; /&gt;
     &lt;xs:enumeration value=&quot;MoveMemberToSibling&quot; /&gt;
     &lt;xs:enumeration value=&quot;AnnotateMember&quot; /&gt;
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
  <p>NotSpecified</p>
  </td>
  <td>
  <p>The type of change is unspecified.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>CreateMember</p>
  </td>
  <td>
  <p>A member was created.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ChangeMemberStatus</p>
  </td>
  <td>
  <p>A member was deactivated or reactivated.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>SetAttributeValue</p>
  </td>
  <td>
  <p>An attribute value of a member was changed.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>MoveMemberToParent</p>
  </td>
  <td>
  <p>A member was moved under a new parent in an explicit
  hierarchy.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>MoveMemberToSibling</p>
  </td>
  <td>
  <p>A member was moved behind a new sibling in an explicit
  hierarchy.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>AnnotateMember</p>
  </td>
  <td>
  <p>An annotation was added to a member record.</p>
  </td>
 </tr>
</table>

<p> </p>


                </div>
            </div>
        </div>
    </body>
</html>