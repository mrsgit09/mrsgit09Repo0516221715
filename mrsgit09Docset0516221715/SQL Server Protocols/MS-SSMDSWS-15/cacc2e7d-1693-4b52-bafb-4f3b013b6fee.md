<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.80.2.2 TransactionsReverseResponse</title>
        <xml>
            <mshelp:toctitle title="3.1.4.80.2.2 TransactionsReverseResponse"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: TransactionsReverseResponse"></mshelp:rltitle>
            <mshelp:keyword index="A" term="cacc2e7d-1693-4b52-bafb-4f3b013b6fee"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="cacc2e7d-1693-4b52-bafb-4f3b013b6fee"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: TransactionsReverseResponse" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.80.2.2 TransactionsReverseResponse</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>TransactionsReverseResponse</b> element provides a
list of the replacement identifiers of the reversed transactions or the
standard operation result.</p>

<p>The following is the XML schema definition of the <b>TransactionsReverseResponse</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xs:element name=&quot;TransactionsReverseResponse&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:complexType&gt;
     &lt;xs:sequence&gt;
       &lt;xs:element xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; minOccurs=&quot;0&quot; name=&quot;OperationResult&quot; nillable=&quot;true&quot; type=&quot;q999:OperationResult&quot; /&gt;
       &lt;xs:element xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; minOccurs=&quot;0&quot; name=&quot;TransactionsReversed&quot; nillable=&quot;true&quot; type=&quot;q999:ArrayOfReplacementId&quot; /&gt;
     &lt;/xs:sequence&gt;
   &lt;/xs:complexType&gt;
 &lt;/xs:element&gt;
</pre></div>
</dd></dl>

<p><b>OperationResult</b>: Specifies the list of errors
that is returned if the operation fails.</p>

<p><b>TransactionsReversed</b>: Specifies the list of
prior and replacement identifiers that identify the transactions that were
reversed.</p>


                </div>
            </div>
        </div>
    </body>
</html>