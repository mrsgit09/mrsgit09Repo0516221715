<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.22 EntityMemberAnnotationsCreate</title>
        <xml>
            <mshelp:toctitle title="3.1.4.22 EntityMemberAnnotationsCreate"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: EntityMemberAnnotationsCreate"></mshelp:rltitle>
            <mshelp:keyword index="A" term="3cf1fcb6-86cb-4ced-be89-8ab932ea80a7"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="3cf1fcb6-86cb-4ced-be89-8ab932ea80a7"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: EntityMemberAnnotationsCreate" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.22 EntityMemberAnnotationsCreate</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>EntityMemberAnnotationsCreate</b> operation adds a
comment that is not associated with a transaction to a member record. In other
words, the comment is a stand-alone annotation, meaning that the annotation is
attached directly to a member and not to a transaction.</p>

<p>This operation MUST include the following elements to create
the annotations: </p>

<ul><li><p><span><span> 
</span></span>EntityId</p>

</li><li><p><span><span> 
</span></span>MemberId</p>

</li><li><p><span><span> 
</span></span>ModelId</p>

</li><li><p><span><span> 
</span></span>VersionId</p>

</li></ul><p>Additionally, at least one annotation MUST be included in a
collection of annotations.</p>

<p>This operation returns an <a href="ffbc22a5-b743-4611-87f6-7527653bcf92.md">AnnotationsCreateResponse</a>
message.</p>

<p>The following is the WSDL definition of the <b>EntityMemberAnnotationsCreate</b>
operation.</p>

<dl>
<dd>
<div><pre> &lt;wsdl:operation name=&quot;EntityMemberAnnotationsCreate&quot; xmlns:wsdl=&quot;http://schemas.xmlsoap.org/wsdl/&quot;&gt;
   &lt;wsdl:input wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/EntityMemberAnnotationsCreate&quot; name=&quot;EntityMemberAnnotationsCreateRequest&quot; message=&quot;tns:EntityMemberAnnotationsCreateRequest&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:output wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/EntityMemberAnnotationsCreateResponse&quot; name=&quot;AnnotationsCreateResponse&quot; message=&quot;tns:AnnotationsCreateResponse&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:fault wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/EntityMemberAnnotationsCreateEditionExpiredMessageFault&quot; name=&quot;EditionExpiredMessageFault&quot; message=&quot;tns:IService_EntityMemberAnnotationsCreate_EditionExpiredMessageFault_FaultMessage&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
   &lt;wsdl:fault wsaw:Action=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09/IService/EntityMemberAnnotationsCreateSkuNotSupportedMessageFault&quot; name=&quot;SkuNotSupportedMessageFault&quot; message=&quot;tns:IService_EntityMemberAnnotationsCreate_SkuNotSupportedMessageFault_FaultMessage&quot; xmlns:wsaw=&quot;http://www.w3.org/2006/05/addressing/wsdl&quot; /&gt;
 &lt;/wsdl:operation&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>