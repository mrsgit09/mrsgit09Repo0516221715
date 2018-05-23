<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.4.101 BusinessRule</title>
        <xml>
            <mshelp:toctitle title="2.2.4.101 BusinessRule"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSMDSWS-15]: BusinessRule"></mshelp:rltitle>
            <mshelp:keyword index="A" term="20edf0db-bc12-4cf8-84b0-bdcfeb77902b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="20edf0db-bc12-4cf8-84b0-bdcfeb77902b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSMDSWS-15]: BusinessRule" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.4.101 BusinessRule</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>BusinessRule</b> complex type specifies a business
rule container object.</p>

<p>The following is the XML schema definition of the <b>BusinessRule</b>
complex type.</p>

<dl>
<dd>
<div><pre> &lt;xs:complexType name=&quot;BusinessRule&quot; xmlns:xs=&quot;http://www.w3.org/2001/XMLSchema&quot;&gt;
   &lt;xs:complexContent mixed=&quot;false&quot;&gt;
     &lt;xs:extension xmlns:q999=&quot;http://schemas.microsoft.com/sqlserver/masterdataservices/2009/09&quot; base=&quot;q999:DataContractBase&quot;&gt;
       &lt;xs:sequence&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;AuditInfo&quot; nillable=&quot;true&quot; type=&quot;q999:AuditInfo&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;BRActions&quot; nillable=&quot;true&quot; type=&quot;q999:ArrayOfBRAction&quot;&gt;
           &lt;xs:annotation&gt;
             &lt;xs:appinfo&gt;
               &lt;DefaultValue xmlns=&quot;http://schemas.microsoft.com/2003/10/Serialization/&quot; EmitDefaultValue=&quot;false&quot; /&gt;
             &lt;/xs:appinfo&gt;
           &lt;/xs:annotation&gt;
         &lt;/xs:element&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;BRConditionTree&quot; nillable=&quot;true&quot; type=&quot;q999:BRConditionTreeNode&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;BRElseActions&quot; nillable=&quot;true&quot; type=&quot;q999:ArrayOfBRAction&quot;&gt;
           &lt;xs:annotation&gt;
             &lt;xs:appinfo&gt;
               &lt;DefaultValue xmlns=&quot;http://schemas.microsoft.com/2003/10/Serialization/&quot; EmitDefaultValue=&quot;false&quot; /&gt;
             &lt;/xs:appinfo&gt;
           &lt;/xs:annotation&gt;
         &lt;/xs:element&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;Description&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;Identifier&quot; nillable=&quot;true&quot; type=&quot;q999:MemberTypeContextIdentifier&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;IsCorrupted&quot; type=&quot;xs:boolean&quot;&gt;
           &lt;xs:annotation&gt;
             &lt;xs:appinfo&gt;
               &lt;DefaultValue xmlns=&quot;http://schemas.microsoft.com/2003/10/Serialization/&quot; EmitDefaultValue=&quot;false&quot; /&gt;
             &lt;/xs:appinfo&gt;
           &lt;/xs:annotation&gt;
         &lt;/xs:element&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;IsFullDefinition&quot; type=&quot;xs:boolean&quot;&gt;
           &lt;xs:annotation&gt;
             &lt;xs:appinfo&gt;
               &lt;DefaultValue xmlns=&quot;http://schemas.microsoft.com/2003/10/Serialization/&quot; EmitDefaultValue=&quot;false&quot; /&gt;
             &lt;/xs:appinfo&gt;
           &lt;/xs:annotation&gt;
         &lt;/xs:element&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;NotificationGroup&quot; nillable=&quot;true&quot; type=&quot;ser:guid&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;NotificationUser&quot; nillable=&quot;true&quot; type=&quot;ser:guid&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;Priority&quot; type=&quot;xs:int&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;RuleActionText&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;RuleConditionText&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;RuleElseActionText&quot; nillable=&quot;true&quot; type=&quot;xs:string&quot; /&gt;
         &lt;xs:element minOccurs=&quot;0&quot; name=&quot;Status&quot; type=&quot;q999:BRStatus&quot; /&gt;
       &lt;/xs:sequence&gt;
     &lt;/xs:extension&gt;
   &lt;/xs:complexContent&gt;
&lt;/xs:complexType&gt;
</pre></div>
</dd></dl>

<p><b>AuditInfo</b>: Specifies the modification history
of the current business rule.</p>

<p><b>BRActions</b>: Specifies the collection of actions
to be performed on the current business rule.</p>

<p><b>BRConditionTree</b>: Specifies the topmost
condition tree node of the business rule.</p>

<p><b>BRElseActions</b>: Specifies the collection of
actions to perform in the ELSE case.</p>

<p><b>Description</b>: Specifies the string that
represents the long description of the current business rule.</p>

<p><b>Identifier</b>: Specifies the unique identifier of
the current business rule.</p>

<p><b>IsCorrupted</b>: Specifies whether the business rule is
corrupted.</p>

<p><b>IsFullDefinition</b>: Specifies whether the business rule
contains a full definition of a business rule.</p>

<p><b>NotificationGroup</b>: Specifies the <a href="ad350219-f30b-4bac-99e5-6477986f9a7a.htm#gt_2bd35dd1-142e-4a80-9ac8-cd7ea05de566">MUID</a> of the group to be
notified about the rule. Either <b>NotificationGroup</b> or <b>NotificationUser</b>
can be specified, but not both.</p>

<p><b>NotificationUser</b>: Specifies the MUID of the
user to be notified about the rule. Either <b>NotificationGroup</b> or <b>NotificationUser</b>
can be specified, but not both.</p>

<p><b>Priority</b>: Specifies an integer that sets the
priority of the business rule.</p>

<p><b>RuleActionText</b>: Specifies a descriptive
representation of business rule actions that are included in the business rule.</p>

<p><b>RuleConditionText</b>: Specifies a text-based
representation of business rule <a href="ad350219-f30b-4bac-99e5-6477986f9a7a.htm#gt_9a1c3bd3-d971-482a-adfe-6f41e427b95f">conditions</a> that are
included in the business rule.</p>

<p><b>Status</b>: Specifies the status of the current
business rule.</p>


                </div>
            </div>
        </div>
    </body>
</html>