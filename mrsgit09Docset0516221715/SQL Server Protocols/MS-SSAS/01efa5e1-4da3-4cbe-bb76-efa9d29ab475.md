<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>4.5.2 Server Response</title>
        <xml>
            <mshelp:toctitle title="4.5.2 Server Response"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: Server Response"></mshelp:rltitle>
            <mshelp:keyword index="A" term="01efa5e1-4da3-4cbe-bb76-efa9d29ab475"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="01efa5e1-4da3-4cbe-bb76-efa9d29ab475"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: Server Response" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">4.5.2 Server Response</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The server responds with a list of mining models:</p>

<dl>
<dd>
<div><pre> &lt;soap:Envelope xmlns:soap=&quot;http://schemas.xmlsoap.org/soap/envelope/&quot;&gt;
   &lt;soap:Body&gt;
     &lt;DiscoverResponse xmlns=&quot;urn:schemas-microsoft-com:xml-analysis&quot; xmlns:ddl2=&quot;http://schemas.microsoft.com/analysisservices/2003/engine/2&quot; xmlns:ddl2_2=&quot;http://schemas.microsoft.com/analysisservices/2003/engine/2/2&quot; xmlns:ddl100=&quot;http://schemas.microsoft.com/analysisservices/2008/engine/100&quot; xmlns:ddl100_100=&quot;http://schemas.microsoft.com/analysisservices/2008/engine/100/100&quot;&gt;
       &lt;return&gt;
         &lt;root xmlns=&quot;urn:schemas-microsoft-com:xml-analysis:rowset&quot; xmlns:xsi=&quot;http://www.w3.org/2001/XMLSchema-instance&quot; xmlns:xsd=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
           &lt;row&gt;
             &lt;MODEL_CATALOG&gt;AdventureWorks_SSAS&lt;/MODEL_CATALOG&gt;
             &lt;MODEL_NAME&gt;Dim Product&lt;/MODEL_NAME&gt;
             &lt;MODEL_GUID&gt;BC9EA693-C163-4609-89F2-FD38A498B43E&lt;/MODEL_GUID&gt;
             &lt;DESCRIPTION /&gt;
             &lt;DATE_CREATED&gt;2009-03-08T08:50:23&lt;/DATE_CREATED&gt;
             &lt;DATE_MODIFIED&gt;2009-03-10T06:53:43&lt;/DATE_MODIFIED&gt;
             &lt;SERVICE_TYPE_ID&gt;1&lt;/SERVICE_TYPE_ID&gt;
             &lt;SERVICE_NAME&gt;Microsoft_Decision_Trees&lt;/SERVICE_NAME&gt;
             &lt;PREDICTION_ENTITY&gt;Sales Amount&lt;/PREDICTION_ENTITY&gt;
             &lt;IS_POPULATED&gt;true&lt;/IS_POPULATED&gt;
             &lt;MINING_PARAMETERS&gt;COMPLEXITY_PENALTY=0.5,MAXIMUM_INPUT_ATTRIBUTES=255,MAXIMUM_OUTPUT_ATTRIBUTES=255,MINIMUM_SUPPORT=10,SCORE_METHOD=4,SPLIT_METHOD=3,FORCE_REGRESSOR=&lt;/MINING_PARAMETERS&gt;
             &lt;MINING_STRUCTURE&gt;Dim Product Mining&lt;/MINING_STRUCTURE&gt;
             &lt;LAST_PROCESSED&gt;2009-03-08T08:50:33&lt;/LAST_PROCESSED&gt;
             &lt;MSOLAP_IS_DRILLTHROUGH_ENABLED&gt;true&lt;/MSOLAP_IS_DRILLTHROUGH_ENABLED&gt;
             &lt;FILTER /&gt;
             &lt;TRAINING_SET_SIZE&gt;354&lt;/TRAINING_SET_SIZE&gt;
           &lt;/row&gt;
         &lt;/root&gt;
       &lt;/return&gt;
     &lt;/DiscoverResponse&gt;
   &lt;/soap:Body&gt;
 &lt;/soap:Envelope&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>