<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.186 PinLabel</title>
        <xml>
            <mshelp:toctitle title="2.186 PinLabel"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: PinLabel"></mshelp:rltitle>
            <mshelp:keyword index="A" term="8a95fbbe-67d8-418f-8b2c-dc7fb18fdf6b"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="8a95fbbe-67d8-418f-8b2c-dc7fb18fdf6b"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: PinLabel" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.186 PinLabel</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b><i>Applies to </i></b><a href="1e855f94-4617-47e4-b89e-0856c6cb420f.html"><b><i>RDL 2008/01</i></b></a><b><i>,
</i></b><a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.html"><b><i>RDL 2010/01</i></b></a><b><i>,
and </i></b><a href="52ce3983-2bfc-4e72-9359-42aaf5fe4509.html"><b><i>RDL 2016/01</i></b></a></p>

<p>The <b>PinLabel</b> element specifies a label for a <a href="b04b7ea8-b15d-4c22-a1e2-c8ac4f7f01b0.html">ScalePin</a>. This element is
optional.</p>

<p>The following are the parent and child elements of the <b>PinLabel</b>
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
  <p>ScalePin</p>
  </td>
 </tr>
</table>

<p> </p>

<table>
 <thead>
  <tr>
   <th>
   <p>Child elements</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="5bb2e66d-9e68-456f-a890-2be21ab8a638.html">PinLabel.AllowUpsideDown</a>
  </p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="d2799a22-6982-4d75-8422-bafd14f5a523.html">PinLabel.DistanceFromScale</a>
  </p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="2d61b0cd-d471-44e9-9169-20804df2bc34.html">PinLabel.FontAngle</a>
  </p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="bb042693-f356-4e70-8294-ed755ef19f8b.html">PinLabel.Placement</a>
  </p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="4239ae8b-8814-4669-8eb3-815757726d60.html">PinLabel.RotateLabel</a>
  </p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="5a5d14e3-4d2e-418f-b955-3608c28056d8.html">PinLabel.Style</a>
  </p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="a540815c-440d-4c54-8ef1-0302c3303266.html">PinLabel.Text</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="2c035bc1-623f-403f-826a-a4cb1ee92bf0.html">PinLabel.UseFontPercent</a></p>
  </td>
 </tr>
</table>

<p>The following is the XML Schema definition of the <b>PinLabel</b>
element in RDL 2008/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;PinLabelType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;Style&quot; type=&quot;StyleType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;Text&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;AllowUpsideDown&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DistanceFromScale&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;FontAngle&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;Placement&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;RotateLabel&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;UseFontPercent&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;skip&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>

<p>The following is the XML Schema definition of the <b>PinLabel</b>
element in RDL 2010/01 and RDL 2016/01.</p>

<dl>
<dd>
<div><pre> &lt;xsd:complexType name=&quot;PinLabelType&quot;&gt;
   &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
     &lt;xsd:element name=&quot;Style&quot; type=&quot;StyleType&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;Text&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;AllowUpsideDown&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;DistanceFromScale&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;FontAngle&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;Placement&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;RotateLabel&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:element name=&quot;UseFontPercent&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
     &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:choice&gt;
   &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
 &lt;/xsd:complexType&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>