<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.183 SystemDomainListGetCriteria</title>
        <xml>
            <mshelp:toctitle title="2.2.4.183 SystemDomainListGetCriteria"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: SystemDomainListGetCriteria"></mshelp:rltitle>
            <mshelp:keyword index="A" term="ec5ab1d2-7fa1-4a26-b0dd-c1fd006f4f6b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="ec5ab1d2-7fa1-4a26-b0dd-c1fd006f4f6b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: SystemDomainListGetCriteria" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.183 SystemDomainListGetCriteria</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>SystemDomainListGetCriteria</b> complex type
specifies the query criteria that determine which domain lists to retrieve. The
parameters that are specified are combined with an AND. To retrieve all
metadata, leave all parameters empty.</p>

<p>The following is the XML schema definition of the <b>SystemDomainListGetCriteria</b>
complex type.</p>

<dl>
<dd>
<div><pre> &lt;xs:complexType name=&quot;SystemDomainListGetCriteria&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:complexContent mixed=&quot;false&quot;&gt;
     &lt;xs:extension xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; base=&quot;q999:DataContractBase&quot;&gt;
       &lt;xs:sequence&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;ListCode&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;ListGroup&quot; nillable=&quot;true&quot; type=&quot;xs:int&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;ListOption&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
       &lt;/xs:sequence&gt;
     &lt;/xs:extension&gt;
   &lt;/xs:complexContent&gt;
 &lt;/xs:complexType&gt;
</pre></div>
</dd></dl>

<p><b>ListCode</b>: Specifies the name of the domain
list on which to filter. When this element is unspecified, all domain lists are
returned.</p>

<p><b>ListGroup</b>: Specifies the individual list
grouping or category on which to filter. When this element is not provided, all
list groups are returned.</p>

<p><b>ListOption</b>: Specifies the individual list
option on which to filter. When this element is unspecified, all list options
are returned.</p>


                </div>
            </div>
        </div>
    </body>
</html>