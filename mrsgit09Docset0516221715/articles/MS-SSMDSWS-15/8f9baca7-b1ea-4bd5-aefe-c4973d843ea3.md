<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.81 UserEffectiveObjectPermissionsGet</title>
        <xml>
            <mshelp:toctitle title="3.1.4.81 UserEffectiveObjectPermissionsGet"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: UserEffectiveObjectPermissionsGet"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8f9baca7-b1ea-4bd5-aefe-c4973d843ea3"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8f9baca7-b1ea-4bd5-aefe-c4973d843ea3"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: UserEffectiveObjectPermissionsGet" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.81 UserEffectiveObjectPermissionsGet</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>UserEffectiveObjectPermissionsGet</b> operation
retrieves a list of users from the Master Data Services (MDS) repository based
on the specified effective object permissions.</p>

<p>The following is the XML schema definition of the <b>UserEffectiveObjectPermissionsGet</b>
operation.</p>

<dl>
<dd>
<div><pre> &lt;wsdl:operation name=&quot;UserEffectiveObjectPermissionsGet&quot; xmlns:wsdl=&quot;http://schemas.xmlsoap.org/wsdl/&quot;&gt;
   &lt;wsdl:input wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserEffectiveObjectPermissionsGet&quot; name=&quot;UserEffectiveObjectPermissionsGetRequest&quot; message=&quot;tns:UserEffectiveObjectPermissionsGetRequest&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:output wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserEffectiveObjectPermissionsGetResponse&quot; name=&quot;UserEffectiveObjectPermissionsGetResponse&quot; message=&quot;tns:UserEffectiveObjectPermissionsGetResponse&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:fault wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserEffectiveObjectPermissionsGetEditionExpiredMessageFault&quot; name=&quot;EditionExpiredMessageFault&quot; message=&quot;tns:IService_UserEffectiveObjectPermissionsGet_EditionExpiredMessageFault_FaultMessage&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:fault wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserEffectiveObjectPermissionsGetSkuNotSupportedMessageFault&quot; name=&quot;SkuNotSupportedMessageFault&quot; message=&quot;tns:Iservice_UserEffectiveObjectPermissionsGet_SkuNotSupportedMessageFault_FaultMessage&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
 &lt;/wsdl:operation&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>