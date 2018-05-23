<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.39 ArrayOfKeyValueOfguidArrayOfguidox8ieOcg</title>
        <xml>
            <mshelp:toctitle title="2.2.4.39 ArrayOfKeyValueOfguidArrayOfguidox8ieOcg"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: ArrayOfKeyValueOfguidArrayOfguidox8ieOcg"></mshelp:rltitle>
            <mshelp:keyword index="A" term="25909bad-cc0c-46b5-aea7-b16a4fdba5a2"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="25909bad-cc0c-46b5-aea7-b16a4fdba5a2"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: ArrayOfKeyValueOfguidArrayOfguidox8ieOcg" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.39 ArrayOfKeyValueOfguidArrayOfguidox8ieOcg</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>ArrayOfKeyValueOfguidArrayOfguidox8ieOcg</b> complex
type specifies a collection of <b>KeyValueOfguidArrayOfguidox8ieOcg </b>complex
types.</p>

<p>The following is the XML schema definition of the <b>ArrayOfKeyValueOfguidArrayOfguidox8ieOcg</b>
complex type.</p>

<dl>
<dd>
<div><pre>   &lt;xs:complexType name=&quot;ArrayOfKeyValueOfguidArrayOfguidox8ieOcg&quot;&gt;
     &lt;xs:sequence&gt;
       &lt;xs:element minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot; name=&quot;KeyValueOfguidArrayOfguidox8ieOcg&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
     &lt;xs:complexType&gt;
       &lt;xs:sequence&gt;
         &lt;xs:element name=&quot;Key&quot; type=&quot;ser:guid&quot; /&gt;
         &lt;xs:element name=&quot;Value&quot; nillable=&quot;true&quot; type=&quot;tns:ArrayOfguid&quot; /&gt;
       &lt;/xs:sequence&gt;
     &lt;/xs:complexType&gt;
       &lt;/xs:element&gt;
     &lt;/xs:sequence&gt;
   &lt;/xs:complexType&gt;
</pre></div>
</dd></dl>

<p><b>KeyValueOfguidArrayOfguidox8ieOcg</b>: Specifies
the <b>KeyValueOfguidArrayOfguidox8ieOcg</b> complex type.</p>


                </div>
            </div>
        </div>
    </body>
</html>