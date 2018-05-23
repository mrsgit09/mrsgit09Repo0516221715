<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.199.16 RadialPointer.NeedleStyle</title>
        <xml>
            <mshelp:toctitle title="2.199.16 RadialPointer.NeedleStyle"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: RadialPointer.NeedleStyle"></mshelp:rltitle>
            <mshelp:keyword index="A" term="2bf22a11-ba0b-489b-bcdd-7a41dc54ff0d"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="2bf22a11-ba0b-489b-bcdd-7a41dc54ff0d"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: RadialPointer.NeedleStyle" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.199.16 RadialPointer.NeedleStyle</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.md"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.md"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.md"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>RadialPointer.NeedleStyle</b> element specifies the
style of a <a href="b2482b3f-74ab-4ca8-a9e5-c07955011743.md#gt_41325275-2cae-4dba-9fde-53833f547fce">radial pointer</a>
needle. This element is optional. This element is ignored if peer element <a href="f85928f8-9c6c-4d7f-876c-db08e412c09c.md">RadialPointer.Type</a> is not
set to &quot;Needle&quot;. </p>

<p>If the <b>RadialPointer.NeedleStyle</b> element is present,
its value MUST be a <a href="1ed81ef3-a683-45e3-aaad-bd2bbe71bc3d.md">String</a>
(<a href="https://go.microsoft.com/fwlink/?LinkId=90610">[XMLSCHEMA2]</a>
section 3.2.1) or an expression that evaluates to a <b>String</b>. The value of
this element MUST be one of the following or an expression that evaluates to
one of the following:</p>

<p><b>Triangular:</b> Specifies that the needle is
shaped like a triangle.</p>

<p><b>Rectangular:</b> Specifies that the needle is
shaped like a rectangle.</p>

<p><b>TaperedWithTail:</b> Specifies that the needle is
tapered and contains a rectangular tail.</p>

<p><b>Tapered:</b> Specifies that the needle is tapered
without a rectangular tail.</p>

<p><b>ArrowWithTail:</b> Specifies that the needle is
shaped like an arrow with a rectangular tail.</p>

<p><b>Arrow:</b> Specifies that the needle is shaped
like an arrow without a rectangular tail.</p>

<p><b>StealthArrowWithTail:</b> Specifies that the
needle is shaped like an arrow with a diagonal tip with a rectangular tail.</p>

<p><b>StealthArrow:</b> Specifies that the needle is
shaped like an arrow with a diagonal tip without a rectangular tail.</p>

<p><b>TaperedWithStealthArrow:</b> Specifies that the
needle is tapered and has a stealth arrow tip.</p>

<p><b>StealthArrowWithWideTail:</b> Specifies that the
needle has a stealth arrow tip and a diagonally widening tail.</p>

<p><b>TaperedWithRoundedPoint:</b> Specifies that the
needle is tapered with a rounded end.</p>

<p>If the <b>RadialPointer.NeedleStyle</b> element is not
present, its value is interpreted as &quot;Triangular&quot;.</p>

<p>The following is the parent element of the <b>RadialPointer.NeedleStyle</b>
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
  <p><a href="1446314e-813e-42f0-9a28-f1b96fd3a0da.md">RadialPointer</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>RadialPointer.NeedleStyle</b>
element.</p>

<dl>
<dd>
<div><pre> &lt;xsd:element name=&quot;NeedleStyle&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>