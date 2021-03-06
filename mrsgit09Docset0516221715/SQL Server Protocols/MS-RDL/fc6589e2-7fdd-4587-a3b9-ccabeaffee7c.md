<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.327.5 Field.AggregateIndicatorField</title>
        <xml>
            <mshelp:toctitle title="2.327.5 Field.AggregateIndicatorField"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: Field.AggregateIndicatorField"></mshelp:rltitle>
            <mshelp:keyword index="A" term="fc6589e2-7fdd-4587-a3b9-ccabeaffee7c"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="fc6589e2-7fdd-4587-a3b9-ccabeaffee7c"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: Field.AggregateIndicatorField" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.327.5 Field.AggregateIndicatorField</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="bf2bab1a-b608-4bcc-b718-1cc1baa9579c.md"><b><i>RDL 2011/01</i></b></a></p>

<p>The <b>Field.AggregateIndicatorField</b> element specifies
the name of another <a href="940b8522-5d1f-4a2a-ab79-087ef6a69881.md">Field</a>
that specifies whether the data is aggregated over the current <b>Field</b>.
The referenced <b>Field</b> MUST evaluate to a <a href="4802fa14-3619-43fa-9898-3acab160a24c.md">Boolean</a> value. If the value
evaluates to true, the data in the current row is aggregated over this field.
If the value evaluates to false the data in the current row is grouped by this
field.</p>

<p>This element is optional. If this element is present, its
value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a>
(<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a>
section 3.2.1) that contains the name of another <b>Field</b> in the same <a href="a14782b0-2e2f-4305-83a3-3de3fd750b6a.md">DataSet</a>.<a id="Appendix_A_Target_173"></a><a href="1fe5fd87-2de5-4b2c-b762-5a4fd1373621.md#Appendix_A_173" aria-label="Product behavior note 173">&lt;173&gt;</a></p>

<p>Following is the parent element of the <b>Field.AggregateIndicatorField</b>
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
  <p>Field</p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>Field.AggregateIndicatorField</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name =&quot;AggregateIndicatorField&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>