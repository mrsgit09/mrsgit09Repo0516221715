<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.199 ValidationProcessResult</title>
        <xml>
            <mshelp:toctitle title="2.2.4.199 ValidationProcessResult"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: ValidationProcessResult"></mshelp:rltitle>
            <mshelp:keyword index="A" term="a97d039f-4238-4fd9-bd2e-f8f3fcdf0dee"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="a97d039f-4238-4fd9-bd2e-f8f3fcdf0dee"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: ValidationProcessResult" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.199 ValidationProcessResult</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>ValidationProcessResult</b> complex type contains
results of the validation process.</p>

<p>The following is the XML schema definition of the <b>ValidationProcessResult</b>
complex type.</p>

<dl>
<dd>
<div><pre> &lt;xs:complexType name=&quot;ValidationProcessResult&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:complexContent mixed=&quot;false&quot;&gt;
     &lt;xs:extension xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; base=&quot;q999:DataContractBase&quot;&gt;
       &lt;xs:sequence&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;MembersInvalidCount&quot; type=&quot;xs:int&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;MembersValidCount&quot; type=&quot;xs:int&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;MembersValidatedCount&quot; type=&quot;xs:int&quot; /&gt;
       &lt;/xs:sequence&gt;
     &lt;/xs:extension&gt;
   &lt;/xs:complexContent&gt;
 &lt;/xs:complexType&gt;
</pre></div>
</dd></dl>

<p><b>MembersInvalidCount</b>: Specifies the number of
members that are invalid.</p>

<p><b>MembersValidatedCount</b>: Specifies the number of
members that are validated.</p>

<p><b>MembersValidCount</b>: Specifies the number of
members that are valid.</p>


                </div>
            </div>
        </div>
    </body>
</html>