<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.36.2.2 EntityMembersUpdateResponse</title>
        <xml>
            <mshelp:toctitle title="3.1.4.36.2.2 EntityMembersUpdateResponse"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: EntityMembersUpdateResponse"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ba55dded-1499-40ed-8cf8-785bdfeb37ca"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ba55dded-1499-40ed-8cf8-785bdfeb37ca"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: EntityMembersUpdateResponse" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.36.2.2 EntityMembersUpdateResponse</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>EntityMembersUpdateResponse</b> element provides only
the standard operation results.</p>

<p>The following is the XML schema definition of the <b>EntityMembersUpdateResponse</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xs:element name=&quot;EntityMembersUpdateResponse&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:complexType&gt;
     &lt;xs:sequence&gt;
       &lt;xs:element xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; minOccurs=&quot;0&quot; name=&quot;OperationResult&quot; nillable=&quot;true&quot; type=&quot;q999:OperationResult&quot; /&gt;
     &lt;/xs:sequence&gt;
   &lt;/xs:complexType&gt;
 &lt;/xs:element&gt;
</pre></div>
</dd></dl>

<p><b>OperationResult</b>: Specifies the list of errors
that is returned if the operation fails.</p>


                </div>
            </div>
        </div>
    </body>
</html>