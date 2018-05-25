<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>1.3 Overview</title>
        <xml>
            <mshelp:toctitle title="1.3 Overview"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-DTYP]: Overview"></mshelp:rltitle>
            <mshelp:keyword index="A" term="32dfc66c-d737-4e1b-b67f-6cf3a5bdefc7"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="32dfc66c-d737-4e1b-b67f-6cf3a5bdefc7"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-DTYP]: Overview" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">1.3 Overview</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>Two types of data structures are specified in this document:
data structures that are specified in terms of the wire format and data
structures that are RPC-marshaled as specified in <mshelp:link keywords="290c38b1-92fe-4229-91e6-4fc376610c15" tabindex="0">[MS-RPCE]</mshelp:link>.
The latter are specified by using the <a href="a66edeb1-52a0-4d64-a93b-2f5c833d7d92.html#gt_73177eec-4092-420f-92c5-60b2478df824">Interface Definition Language
(IDL)</a> that is defined in [MS-RPCE] section <mshelp:link keywords="5e8b6109-5122-450c-8c00-4b98f3cdb435" tabindex="0">2.2.4</mshelp:link>.</p>

<p>For some types of data, both formats are shown. For example,
both formats are shown if some protocols use the raw wire format but other
protocols use the RPC-marshaled format. Any protocol that uses a data structure
name in its IDL necessarily implies the use of the IDL version of the data
structure. Any other use implies the use of the wire format version unless
otherwise specified by the protocol that uses the data structure.</p>


                </div>
            </div>
        </div>
    </body>
</html>