<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.5.4.2 IdnToUnicode</title>
        <xml>
            <mshelp:toctitle title="3.1.5.4.2 IdnToUnicode"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-UCODEREF]: IdnToUnicode"></mshelp:rltitle>
            <mshelp:keyword index="A" term="3f6eb50d-a7cf-4db6-8ca3-d412dc2d2b1a"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="3f6eb50d-a7cf-4db6-8ca3-d412dc2d2b1a"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-UCODEREF]: IdnToUnicode" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.5.4.2 IdnToUnicode</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<dl>
<dd>
<div><pre> COMMENT IdnToUnicode
 COMMENT  On Entry:  SourceString – Idn String to get Unicode
 COMMENT                            representation of.
 COMMENT             Flags        - Bit flags to control behavior
 COMMENT                            of IDN validation
 COMMENT
 COMMENT  IDN_ALLOW_UNASSIGNED:     During validation, allow unicode
 COMMENT                            code points that are not assigned.   
 COMMENT  IDN_USE_STD3_ASCII_RULES: Enforce validation of the STD3
 COMMENT                            characters.
 COMMENT  IDN_RAW_PUNYCODE:         Only decode the punycode, no additional
 COMMENT                            validation.
 COMMENT  IDN_EMAIL_ADDRESS:        Allow punycode encoding of the local part
 COMMENT                            of an email address to tunnel EAI
 COMMENT                            addresses through non-Unicode slots.
 COMMENT
 COMMENT  On Exit:  UnicodeString - String containing the Unicode form of the
 COMMENT                            input string.
 PROCEDURE IdnToUnicode (IN SourceString : Punycode String,
                         IN Flags: 32 bit integer,
                         OUT UnicodeString : Unicode String)
 UnicodeString = PunycodeDecode(SourceString)
  
 COMMENT IDN_RAW_PUNYCODE stops here
 IF (IDN_RAW_PUNYCODE bit is on in Flags) THEN
     return UnicodeString
 ENDIF
 COMMENT Otherwise verify that the result round trips
 RoundTripPunycodeString = IdnToAscii(UnicodeString, Flags)
 IF (RoundTripPunycodeString IS NOT EQUAL TO UnicodeString)
     return ERROR
 ENDIF
 return UnicodeString
  
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>