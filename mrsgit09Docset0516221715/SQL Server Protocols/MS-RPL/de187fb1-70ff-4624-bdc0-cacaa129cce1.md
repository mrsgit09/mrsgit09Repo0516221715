<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.2.27 Action</title>
        <xml>
            <mshelp:toctitle title="2.2.27 Action"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RPL]: Action"></mshelp:rltitle>
            <mshelp:keyword index="A" term="de187fb1-70ff-4624-bdc0-cacaa129cce1"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="de187fb1-70ff-4624-bdc0-cacaa129cce1"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RPL]: Action" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.2.27 Action</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The <b>Action</b> record specifies the properties of an <a href="75ae48f7-746b-4b41-919c-6699fa28b3ef.html#gt_b178b6c0-7df9-4107-95ca-12c7f0b9900b">action</a>.           </p>

<dl>
<dd>
<div><pre> Action = actionStart actionInfoProperties delimiter
</pre></div>
</dd></dl>

<table>
 <tr>
  <th><p><br>0</p></th>
  <th><p><br>1</p></th>
  <th><p><br>2</p></th>
  <th><p><br>3</p></th>
  <th><p><br>4</p></th>
  <th><p><br>5</p></th>
  <th><p><br>6</p></th>
  <th><p><br>7</p></th>
  <th><p><br>8</p></th>
  <th><p><br>9</p></th>
  <th><p>1<br>0</p></th>
  <th><p><br>1</p></th>
  <th><p><br>2</p></th>
  <th><p><br>3</p></th>
  <th><p><br>4</p></th>
  <th><p><br>5</p></th>
  <th><p><br>6</p></th>
  <th><p><br>7</p></th>
  <th><p><br>8</p></th>
  <th><p><br>9</p></th>
  <th><p>2<br>0</p></th>
  <th><p><br>1</p></th>
  <th><p><br>2</p></th>
  <th><p><br>3</p></th>
  <th><p><br>4</p></th>
  <th><p><br>5</p></th>
  <th><p><br>6</p></th>
  <th><p><br>7</p></th>
  <th><p><br>8</p></th>
  <th><p><br>9</p></th>
  <th><p>3<br>0</p></th>
  <th><p><br>1</p></th>
 </tr>
 <tr>
  <td colspan="8">
  <p>actionStart</p>
  </td>
  <td colspan="24">
  <p>actionInfoProperties
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="8">
  <p>delimiter</p>
  </td>
  
 </tr>
</table>

<p><b>actionStart (1 byte): </b>A byte that specifies
the start of the <b>Action</b> record. The value of the <b>actionStart</b>
field MUST be 0x03.</p>

<p><b>actionInfoProperties (variable): </b>A collection
of structures that specifies the properties applicable to the <b>Action</b>
record. The order of the structures in the collection is arbitrary. The <b>actionInfoProperties</b>
collection can be empty. Each structure contained in the <b>actionInfoProperties</b>
collection MUST be one of the following:</p>

<dl>
<dd>
<table>
 <thead>
  <tr>
   <th>
   <p>Property</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p><a href="07e6d2f5-45d1-415f-b4d0-ed2de8bd7801.html">Label</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="1514971f-28f3-48f8-988d-944eb12799b1.html">HyperLink</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="b7ec7c0d-784a-4a59-bc88-7df07f172b49.html">BookmarkLink</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="b0715db2-0dab-436c-9e30-196ca4e0ccd2.html">DrillthroughId</a></p>
  </td>
 </tr>
 <tr>
  <td>
  <p><a href="b1e1d7c4-3704-4c13-ab66-a781fb598961.html">DrillthroughUrl</a></p>
  </td>
 </tr>
</table>
</dd>
<dd>
<p>If an <b>ActionInfoProperties</b> collection
contains a <b>HyperLink</b> structure, it MUST NOT contain a <b>BookmarkLink</b>,
<b>DrillthroughUrl</b>, or <b>DrillthroughId</b> structure.</p>
</dd>
<dd>
<p>If an <b>ActionInfoProperties</b> collection
contains a <b>BookmarkLink</b> structure, it MUST NOT contain a <b>DrillthroughUrl</b> structure
or a <b>DrillthroughId</b> structure.</p>
</dd>
<dd>
<p>If an <b>ActionInfoProperties</b> collection
contains a <b>DrillthroughUrl</b> structure, it MUST contain a <b>DrillthroughId</b> structure.</p>
</dd>
<dd>
<p>If an <b>ActionInfoProperties</b> collection
contains a <b>DrillthroughId</b> structure, it MUST contain a <b>DrillthroughUrl</b> structure.</p>
</dd></dl>









<p><b>delimiter (1 byte): </b>A byte that specifies the
end of the <b>Action</b> record. The value of the <b>delimiter</b> field MUST
be 0xFF.</p>


                </div>
            </div>
        </div>
    </body>
</html>