<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.4.4.3 ACCESS_ALLOWED_OBJECT_ACE</title>
        <xml>
            <mshelp:toctitle title="2.4.4.3 ACCESS_ALLOWED_OBJECT_ACE"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-DTYP]: ACCESS_ALLOWED_OBJECT_ACE"></mshelp:rltitle>
            <mshelp:keyword index="A" term="c79a383c-2b3f-4655-abe7-dcbb7ce0cfbe"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="c79a383c-2b3f-4655-abe7-dcbb7ce0cfbe"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-DTYP]: ACCESS_ALLOWED_OBJECT_ACE" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.4.4.3 ACCESS_ALLOWED_OBJECT_ACE</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The ACCESS_ALLOWED_OBJECT_ACE structure defines an ACE that
controls allowed access to an object, a property set, or property. The ACE
contains a set of access rights, a <a href="a66edeb1-52a0-4d64-a93b-2f5c833d7d92.html#gt_f49694cc-c350-462d-ab8e-816f0103c6c1">GUID</a> that identifies the
type of object, and a <a href="78eb9013-1c3a-4970-ad1f-2b1dad588a25.html">SID</a>
that identifies the trustee to whom the system will grant access. The ACE also
contains a GUID and a set of flags that control inheritance of the ACE by child
objects.</p>

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
  <p>Flags</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>ObjectType
  (16 bytes)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>InheritedObjectType
  (16 bytes)</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
  </td>
 </tr>
 <tr>
  <td colspan="32">
  <p>...</p>
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
</table>

<p><b>Header (4 bytes): </b>An <a href="628ebb1d-c509-4ea0-a10f-77ef97ca4586.html">ACE_HEADER</a> structure that
specifies the size and type of ACE. It also contains flags that control
inheritance of the ACE by child objects.</p>

<p><b>Mask (4 bytes): </b>An <a href="7a53f60e-e730-4dfe-bbe9-b21b62eb790b.html">ACCESS_MASK</a> that specifies
the user rights allowed by this ACE.</p>

<dl>
<dd>
<table>
 <thead>
  <tr>
   <th>
   <p>Value</p>
   </th>
   <th>
   <p>Meaning</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>ADS_RIGHT_DS_CONTROL_ACCESS</p>
  <p>0X00000100</p>
  </td>
  <td>
  <p>The <b>ObjectType</b> GUID identifies an extended
  access right.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ADS_RIGHT_DS_CREATE_CHILD</p>
  <p>0X00000001</p>
  </td>
  <td>
  <p>The <b>ObjectType</b> GUID identifies a type of child
  object. The ACE controls the trustee's right to create this type of child
  object.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ADS_RIGHT_DS_DELETE_CHILD</p>
  <p>0X00000002</p>
  </td>
  <td>
  <p>The <b>ObjectType</b> GUID identifies a type of child
  object. The ACE controls the trustee's right to delete this type of child
  object.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ADS_RIGHT_DS_READ_PROP</p>
  <p>0x00000010</p>
  </td>
  <td>
  <p>The <b>ObjectType</b> GUID identifies a property set
  or property of the object. The ACE controls the trustee's right to read the
  property or property set.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ADS_RIGHT_DS_WRITE_PROP</p>
  <p>0x00000020</p>
  </td>
  <td>
  <p>The <b>ObjectType</b> GUID identifies a property set
  or property of the object. The ACE controls the trustee's right to write the
  property or property set.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ADS_RIGHT_DS_SELF</p>
  <p>0x00000008</p>
  </td>
  <td>
  <p>The <b>ObjectType</b> GUID identifies a validated
  write.</p>
  </td>
 </tr>
</table>
</dd></dl>

<p><b>Flags  (4 bytes): </b>A 32-bit unsigned integer
that specifies a set of bit flags that indicate whether the <b>ObjectType</b>
and <b>InheritedObjectType</b> fields contain valid data. This parameter can be
one or more of the following values.</p>

<dl>
<dd>
<table>
 <thead>
  <tr>
   <th>
   <p>Value</p>
   </th>
   <th>
   <p>Meaning</p>
   </th>
  </tr>
 </thead>
 <tr>
  <td>
  <p>0x00000000</p>
  </td>
  <td>
  <p>Neither <b>ObjectType</b> nor <b>InheritedObjectType</b>
  are valid.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ACE_OBJECT_TYPE_PRESENT</p>
  <p>0x00000001</p>
  </td>
  <td>
  <p><b>ObjectType</b> is valid.</p>
  </td>
 </tr>
 <tr>
  <td>
  <p>ACE_INHERITED_OBJECT_TYPE_PRESENT</p>
  <p>0x00000002</p>
  </td>
  <td>
  <p><b>InheritedObjectType</b> is valid. If this value is
  not specified, all types of child objects can inherit the ACE.</p>
  </td>
 </tr>
</table>
</dd></dl>

<p><b>ObjectType (16 bytes): </b>A GUID that identifies
a property set, property, extended right, or type of child object. The purpose
of this GUID depends on the user rights specified in the <b>Mask</b> field.
This field is valid only if the ACE _OBJECT_TYPE_PRESENT bit is set in the <b>Flags</b>
field. Otherwise, the <b>ObjectType</b> field is ignored. For information on
access rights and for a mapping of the control access rights to the corresponding
GUID value that identifies each right, see <mshelp:link keywords="d2435927-0999-4c62-8c6d-13ba31a52e1a" tabindex="0">[MS-ADTS]</mshelp:link>
sections <mshelp:link keywords="990fb975-ab31-4bc1-8b75-5da132cd4584" tabindex="0">5.1.3.2</mshelp:link>
and <mshelp:link keywords="1522b774-6464-41a3-87a5-1e5633c3fbbb" tabindex="0">5.1.3.2.1</mshelp:link>.</p>

<p>ACCESS_MASK bits are not mutually exclusive. Therefore, the <b>ObjectType</b>
field can be set in an <a href="d06e5a81-176e-46c6-9cf7-9137aad4455e.html">ACE</a>
with any ACCESS_MASK. If the AccessCheck algorithm calls this ACE and does not
find an appropriate GUID, then that ACE will be ignored. For more information
on access checks and object access, see [MS-ADTS] section <mshelp:link keywords="3da5080d-de25-4ac8-9f2b-982709253dfb" tabindex="0">5.1.3.3.3</mshelp:link>.</p>

<p><b>InheritedObjectType (16 bytes): </b>A GUID that
identifies the type of child object that can inherit the ACE. Inheritance is
also controlled by the inheritance flags in the ACE_HEADER, as well as by any
protection against inheritance placed on the child objects. This field is valid
only if the ACE_INHERITED_OBJECT_TYPE_PRESENT bit is set in the Flags member.
Otherwise, the <b>InheritedObjectType</b> field is ignored.</p>

<p><b>Sid (variable): </b>The SID of a trustee. The
length of the SID MUST be a multiple of 4.</p>


                </div>
            </div>
        </div>
    </body>
</html>