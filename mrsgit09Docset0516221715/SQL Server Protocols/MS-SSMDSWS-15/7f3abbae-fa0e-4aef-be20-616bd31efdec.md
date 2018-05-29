<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.78 BRActionGroup</title>
        <xml>
            <mshelp:toctitle title="2.2.4.78 BRActionGroup"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: BRActionGroup"></mshelp:rltitle>
            <mshelp:keyword index="A" term="7f3abbae-fa0e-4aef-be20-616bd31efdec"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="7f3abbae-fa0e-4aef-be20-616bd31efdec"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: BRActionGroup" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.78 BRActionGroup</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>BRActionGroup</b> complex type specifies a grouping
of related <a href="ad350219-f30b-4bac-99e5-6477986f9a7a.html#gt_b677f217-1682-44fc-9507-ca91e09123ef">business rule</a>
action components that are currently available for use in MDS.</p>

<p>The following is the XML schema definition of the <b>BRActionGroup</b>
complex type.</p>

<dl>
<dd>
<div><pre> &lt;xs:complexType name=&quot;BRActionGroup&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:complexContent mixed=&quot;false&quot;&gt;
     &lt;xs:extension xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; base=&quot;q999:DataContractBase&quot;&gt;
       &lt;xs:sequence&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;BRActionComponents&quot; nillable=&quot;true&quot; type=&quot;q999:ArrayOfBRActionComponent&quot;&gt;
           &lt;xs:annotation&gt;
             &lt;xs:appinfo&gt;
               &lt;DefaultValue xmlns=&quot;http://schemas.microsoft.com/2003/10/Serialization/&quot; EmitDefaultValue=&quot;false&quot; /&gt;
             &lt;/xs:appinfo&gt;
           &lt;/xs:annotation&gt;
         &lt;/xs:element&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;Name&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
       &lt;/xs:sequence&gt;
     &lt;/xs:extension&gt;
   &lt;/xs:complexContent&gt;
 &lt;/xs:complexType&gt;
</pre></div>
</dd></dl>

<p><b>BRActionComponents</b>: Specifies a collection of
business rule action components.</p>

<p><b>Name</b>: Specifies the name of the group of
action components.</p>


                </div>
            </div>
        </div>
    </body>
</html>