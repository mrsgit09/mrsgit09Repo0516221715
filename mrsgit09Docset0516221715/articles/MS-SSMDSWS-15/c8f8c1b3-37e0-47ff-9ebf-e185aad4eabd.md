<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.82 UserPreferencesDelete</title>
        <xml>
            <mshelp:toctitle title="3.1.4.82 UserPreferencesDelete"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: UserPreferencesDelete"></mshelp:rltitle>
            <mshelp:keyword index="A" term="c8f8c1b3-37e0-47ff-9ebf-e185aad4eabd"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="c8f8c1b3-37e0-47ff-9ebf-e185aad4eabd"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: UserPreferencesDelete" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.82 UserPreferencesDelete</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>UserPreferencesDelete</b> operation deletes the
current user's selected preferences within the MDS repository. One or more
preferences can be specified for deletion by submitting a dictionary list. This
operation deletes all saved preferences by setting <b>DeleteAllUserPreferences</b>
to &quot;true&quot;.</p>

<p>The following is the WSDL definition of the <b>UserPreferencesDelete</b>
operation.</p>

<dl>
<dd>
<div><pre> &lt;wsdl:operation name=&quot;UserPreferencesDelete&quot; xmlns:wsdl=&quot;http://schemas.xmlsoap.org/wsdl/&quot;&gt;
   &lt;wsdl:input wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserPreferencesDelete&quot; name=&quot;UserPreferencesDeleteRequest&quot; message=&quot;tns:UserPreferencesDeleteRequest&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:output wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserPreferencesDeleteResponse&quot; name=&quot;UserPreferencesDeleteResponse&quot; message=&quot;tns:UserPreferencesDeleteResponse&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:fault wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserPreferencesDeleteSkuNotSupportedMessageFault&quot; name=&quot;SkuNotSupportedMessageFault&quot; message=&quot;tns:IService_UserPreferencesDelete_SkuNotSupportedMessageFault_FaultMessage&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:fault wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/UserPreferencesDeleteEditionExpiredMessageFault&quot; name=&quot;EditionExpiredMessageFault&quot; message=&quot;tns:IService_UserPreferencesDelete_EditionExpiredMessageFault_FaultMessage&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
 &lt;/wsdl:operation&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>