<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.176.2 CustomLabel.AllowUpsideDown</title>
        <xml>
            <mshelp:toctitle title="2.176.2 CustomLabel.AllowUpsideDown"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: CustomLabel.AllowUpsideDown"></mshelp:rltitle>
            <mshelp:keyword index="A" term="6a66989f-4f29-4ff8-8f2c-ddc0acdf4bfc"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="6a66989f-4f29-4ff8-8f2c-ddc0acdf4bfc"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: CustomLabel.AllowUpsideDown" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.176.2 CustomLabel.AllowUpsideDown</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>CustomLabel.AllowUpsideDown</b> element specifies
whether a <a href="519139e8-6188-4286-b148-dfd76a0a6be4.md">CustomLabel</a>
can be rotated by more than 90 degrees. The <b>CustomLabel.AllowUpsideDown</b>
element is optional. </p>

<p>If this element is present, its value MUST be a <a href="4802fa14-3619-43fa-9898-3acab160a24c.md">Boolean</a> (<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a> section
3.2.2) or an expression that evaluates to a <b>Boolean</b>. If this element is
not present, its value is interpreted as false. If the containing element for
this <b>CustomLabel</b> is not a <a href="86468d9f-c561-4b50-a689-5dfccfde8495.md">RadialScale</a>, the <b>CustomLabel.AllowUpsideDown</b>
element is ignored.</p>

<p>The following is the parent element of the <b>CustomLabel.AllowUpsideDown</b>
element.</p>

<table>
 <thead>
  <tr>
   <th>
   <p>Parent elements</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>CustomLabel</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>CustomLabel.AllowUpsideDown</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;AllowUpsideDown&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>