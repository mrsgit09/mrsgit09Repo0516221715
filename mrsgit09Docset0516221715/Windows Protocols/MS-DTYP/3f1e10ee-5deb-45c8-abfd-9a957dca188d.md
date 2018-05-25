<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>2.5.3.1.10 PopStack</title>
        <xml>
            <mshelp:toctitle title="2.5.3.1.10 PopStack"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-DTYP]: PopStack"></mshelp:rltitle>
            <mshelp:keyword index="A" term="3f1e10ee-5deb-45c8-abfd-9a957dca188d"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="3f1e10ee-5deb-45c8-abfd-9a957dca188d"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-DTYP]: PopStack" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">2.5.3.1.10 PopStack</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>A support function, <b>PopStack</b>, pops the topmost
operand from the stack.</p>

<dl>
<dd>
<div><pre> STACKELEMENT
 PopStack (
       STACK ResultStack,
       INT32 StackPos
    )
     --
     -- On entry
     --    ResultStack is the stack.
     --    StackPos is the stack position
  
     IF StackPos equals 0 THEN
        Return NULL
     END IF
  
     Decrement StackPos by 1
     Return ResultStack[StackPos]
 END-SUBROUTINE
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>