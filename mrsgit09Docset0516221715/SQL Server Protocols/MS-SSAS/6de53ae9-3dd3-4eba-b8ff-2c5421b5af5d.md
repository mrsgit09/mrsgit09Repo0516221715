<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.4.3.2.1.1 Command Element</title>
        <xml>
            <mshelp:toctitle title="3.1.4.3.2.1.1 Command Element"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS]: Command Element"></mshelp:rltitle>
            <mshelp:keyword index="A" term="6de53ae9-3dd3-4eba-b8ff-2c5421b5af5d"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="6de53ae9-3dd3-4eba-b8ff-2c5421b5af5d"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS]: Command Element" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.4.3.2.1.1 Command Element</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Command</b> element contains one of the available
commands that can be sent to the server.</p>

<dl>
<dd>
<div><pre>   &lt;xsd:complexType name=&quot;Command&quot;&gt;
     &lt;xsd:choice&gt;
       &lt;xsd:element name=&quot;Statement&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Create&quot; type=&quot;Create&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Alter&quot; type=&quot;Alter&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Delete&quot; type=&quot;Delete&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Process&quot; type=&quot;Process&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;MergePartitions&quot; type=&quot;MergePartitions&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;DesignAggregations&quot; type=&quot;DesignAggregations&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;ClearCache&quot; type=&quot;ClearCache&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Subscribe&quot; type=&quot;Subscribe&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Cancel&quot; type=&quot;Cancel&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;BeginTransaction&quot; type=&quot;BeginTransaction&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;CommitTransaction&quot; type=&quot;CommitTransaction&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;RollbackTransaction&quot; type=&quot;RollbackTransaction&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Lock&quot; type=&quot;Lock&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Unlock&quot; type=&quot;Unlock&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Backup&quot; type=&quot;Backup&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Restore&quot; type=&quot;Restore&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Synchronize&quot; type=&quot;Synchronize&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Attach&quot; type=&quot;Attach&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Detach&quot; type=&quot;Detach&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Insert&quot; type=&quot;Insert&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Update&quot; type=&quot;Update&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Drop&quot; type=&quot;Drop&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;UpdateCells&quot; type=&quot;UpdateCells&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;NotifyTableChange&quot; type=&quot;NotifyTableChange&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;Batch&quot; type=&quot;Batch&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;ImageLoad&quot; type=&quot;ImageLoad&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;ImageSave&quot; type=&quot;ImageSave&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;CloneDatabase&quot; type=&quot;CloneDatabase&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;SetAuthContext&quot; type=&quot;SetAuthContext&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;DBCC&quot; type=&quot;DBCC&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;/xsd:choice&gt;
   &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following subsections define the types for all of the
commands.</p>

<p>In addition to the above commands, <mshelp:link keywords="f85cd3b9-690c-4bc7-a1f0-a854d7daecd8" tabindex="0">[MS-SSAS-T]</mshelp:link>
extends the allowed commands to support databases in Tabular mode with a
compatibility level greater than or equal to 1200.</p>


                </div>
            </div>
        </div>
    </body>
</html>