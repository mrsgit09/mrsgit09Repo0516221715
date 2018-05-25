<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.4.4.7 ACCESS_DENIED_CALLBACK_ACE</title>
        <xml>
            <mshelp:toctitle title="2.4.4.7 ACCESS_DENIED_CALLBACK_ACE"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-DTYP]: ACCESS_DENIED_CALLBACK_ACE"></mshelp:rltitle>
            <mshelp:keyword index="A" term="35adad6b-fda5-4cc1-b1b5-9beda5b07d2e"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="35adad6b-fda5-4cc1-b1b5-9beda5b07d2e"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-DTYP]: ACCESS_DENIED_CALLBACK_ACE" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.4.4.7 ACCESS_DENIED_CALLBACK_ACE</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The ACCESS_DENIED_CALLBACK_ACE structure defines an ACE for
the DACL that controls access to an object. An access-denied ACE denies access
to an object for a specific trustee identified by a <a href="78eb9013-1c3a-4970-ad1f-2b1dad588a25.html">SID</a>.</p>

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
  <td colspan="32">
  <p>Header</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>Mask</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>Sid
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>ApplicationData
  (variable)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
</table>

<p><b>Header (4 bytes): </b>An <a href="628ebb1d-c509-4ea0-a10f-77ef97ca4586.html">ACE_HEADER</a> structure that
specifies the size and type of ACE. It also contains flags that control
inheritance of the ACE by child objects.</p>

<p><b>Mask (4 bytes): </b>An <a href="7a53f60e-e730-4dfe-bbe9-b21b62eb790b.html">ACCESS_MASK</a> that specifies
the user rights denied by this ACE.</p>

<p><b>Sid (variable): </b>The SID of a trustee. The
length of the SID MUST be a multiple of 4.</p>

<p><b>ApplicationData (variable): </b>Optional
application data. The size of the application data is determined by the <b>AceSize</b>
field of the ACE_HEADER.</p>


                </div>
            </div>
        </div>
    </body>
</html>