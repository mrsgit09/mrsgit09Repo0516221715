<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>3.1.7.1 Network Connection Is Disconnected or Encounters Error</title>
        <xml>
            <mshelp:toctitle title="3.1.7.1 Network Connection Is Disconnected or Encounters Error"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSAS8]: Network Connection Is Disconnected or Encounters Error"></mshelp:rltitle>
            <mshelp:keyword index="A" term="78c1ede6-685f-433a-aff2-a6daba40ceac"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="78c1ede6-685f-433a-aff2-a6daba40ceac"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSAS8]: Network Connection Is Disconnected or Encounters Error" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">3.1.7.1 Network Connection Is Disconnected or Encounters Error</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>A client terminates the session by closing the network
connection, without sending a request to the server. The server will then
detect that the TCP connection has been dropped and will clean the state
associated with this connection.</p>

<p>If the client discovers any network errors, it SHOULD<a id="Appendix_A_Target_29"></a><a href="05c9e5c4-4566-418c-a56e-69fca8d73f4b.htm#Appendix_A_29" aria-label="Product behavior note 29">&lt;29&gt;</a> propagate the error to the
higher level application and close the network connection. If time remains for
the high-level operation the client MAY try reconnecting and retrying the
failed operation. </p>


                </div>
            </div>
        </div>
    </body>
</html>