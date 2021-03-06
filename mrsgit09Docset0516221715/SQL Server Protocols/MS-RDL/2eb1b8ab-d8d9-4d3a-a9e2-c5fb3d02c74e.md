<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.337.3 JoinCondition.SortDirection</title>
        <xml>
            <mshelp:toctitle title="2.337.3 JoinCondition.SortDirection"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: JoinCondition.SortDirection"></mshelp:rltitle>
            <mshelp:keyword index="A" term="2eb1b8ab-d8d9-4d3a-a9e2-c5fb3d02c74e"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="2eb1b8ab-d8d9-4d3a-a9e2-c5fb3d02c74e"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: JoinCondition.SortDirection" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.337.3 JoinCondition.SortDirection</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.md"><b><i>RDL 2011/01</i></b></a></p>

<p>The <b>JoinCondition.SortDirection</b> element specifies the
sort order of the <a href="64091774-c185-49ed-821c-9e720b2ee019.md">JoinCondition</a>
element. The <b>JoinCondition.SortDirection</b> element is optional and MUST
NOT be specified more than once. If the <b>JoinCondition</b> has a containing <a href="6d1c77e5-1573-4ad6-8d2a-c507411ad94b.md">Relationship</a>, <b>JoinCondition.SortDirection</b>
MUST NOT be specified unless <a href="010c596a-95a7-4db2-b1e0-76f2d4eb4c7a.md">Relationship.NaturalJoin</a>
is true. If the <b>JoinCondition</b> has a containing <a href="9fa528f6-2956-4f90-98c8-831aeb45aa26.md">DefaultRelationship</a>, <b>JoinCondition.SortDirection</b>
MUST NOT be specified unless <b>DefaultRelationship.NaturalJoin</b> is true. If
the <b>JoinCondition.SortDirection</b> element is specified, its value MUST be
one of the following:</p>

<p><b>Ascending</b> (default): Both <a href="8a8301cb-c9b3-48ca-84fb-03e8724f959f.md">DataSets</a> involved in the <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_b837a3f6-40e2-4181-b82f-badccf629ff7">data correlation</a> are sorted
in ascending order by the <b>JoinCondition</b>.</p>

<p><b>Descending</b>: Both <b>DataSets</b> involved in
the data correlation are sorted in descending order by the <b>JoinCondition</b>.</p>

<p>If the <b>JoinCondition.SortDirection</b> element is not
specified, its value is interpreted as &quot;Ascending&quot;.</p>

<p>Following is the parent element of the <b>JoinCondition.SortDirection</b>
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
  <p>JoinCondition</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>JoinCondition.SortDirection</b>
element.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:element name=&quot;SortDirection&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
     &lt;xsd:simpleType&gt;
       &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
         &lt;xsd:enumeration value=&quot;Ascending&quot;/&gt;
         &lt;xsd:enumeration value=&quot;Descending&quot;/&gt;
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