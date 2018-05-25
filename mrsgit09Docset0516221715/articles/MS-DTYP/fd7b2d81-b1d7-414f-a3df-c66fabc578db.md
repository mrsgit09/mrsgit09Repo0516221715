<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.3.8 MULTI_SZ</title>
        <xml>
            <mshelp:toctitle title="2.3.8 MULTI_SZ"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-DTYP]: MULTI_SZ"></mshelp:rltitle>
            <mshelp:keyword index="A" term="fd7b2d81-b1d7-414f-a3df-c66fabc578db"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="fd7b2d81-b1d7-414f-a3df-c66fabc578db"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-DTYP]: MULTI_SZ" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.3.8 MULTI_SZ</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>The MULTI_SZ structure defines an implementation-specific<a id="Appendix_A_Target_2"></a><a href="11e1608c-6169-4fbc-9c33-373fc9b224f4.html#Appendix_A_2" aria-label="Product behavior note 2">&lt;2&gt;</a> type that contains a sequence of
null-terminated strings, terminated by an empty string (\0) so that the last
two characters are both null terminators.</p>

<dl>
<dd>
<div><pre> typedef struct _MULTI_SZ {
   wchar_t* Value;
   DWORD nChar;
 } MULTI_SZ;
</pre></div>
</dd></dl>

<p><b>Value:</b>  A data buffer, which is a
string literal containing multiple null-terminated strings serially.</p>

<p><b>nChar:</b>  The length, in characters,
including the two terminating nulls.</p>


                </div>
            </div>
        </div>
    </body>
</html>