<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.76.2.2 SystemSettingsUpdateResponse</title>
        <xml>
            <mshelp:toctitle title="3.1.4.76.2.2 SystemSettingsUpdateResponse"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: SystemSettingsUpdateResponse"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ecb28ebb-a7bc-419b-bf31-e3e8f62897ec"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ecb28ebb-a7bc-419b-bf31-e3e8f62897ec"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: SystemSettingsUpdateResponse" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.76.2.2 SystemSettingsUpdateResponse</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>SystemSettingsUpdateResponse</b> element specifies
only standard operation results.</p>

<p>The following is the XML schema definition of the <b>SystemSettingsUpdateResponse</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xs:element name=&quot;SystemSettingsUpdateResponse&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
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