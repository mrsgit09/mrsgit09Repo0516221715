<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>1.1 Glossary</title>
        <xml>
            <mshelp:toctitle title="1.1 Glossary"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-SSNWS]: Glossary"></mshelp:rltitle>
            <mshelp:keyword index="A" term="4baedaec-b5a7-4176-be88-e1cec659ab8c"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="4baedaec-b5a7-4176-be88-e1cec659ab8c"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-SSNWS]: Glossary" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">1.1 Glossary</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p>This document uses the following terms:</p>

<p><a id="gt_108a1419-49a9-4d19-b6ca-7206aa726b3f" /><b>attribute</b>: A
characteristic of some object or entity, typically encoded as a name/value
pair.</a></p>

<p><a id="gt_8e961bf0-95ba-4f58-9034-b67ccb27f317" /><b>authentication</b>: The act
of proving an identity to a server while providing key material that binds the
identity to subsequent communications.</a></p>

<p><a id="gt_648a4ade-ef54-445a-aaa5-c6883b33b20d" /><b>Basic</b>: An authentication
access type supported by HTTP as defined by </a><a href="https://go.microsoft.com/fwlink/?LinkId=90373">[RFC2617]</a>.</p>

<p><a id="gt_7a0f4b71-23ba-434f-b781-28053ed64879" /><b>certificate</b>: A
certificate is a collection of </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_108a1419-49a9-4d19-b6ca-7206aa726b3f">attributes</a> and extensions
that can be stored persistently. The set of attributes in a certificate can
vary depending on the intended usage of the certificate. A certificate securely
binds a public key to the entity that holds the corresponding private key. A
certificate is commonly used for <a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_8e961bf0-95ba-4f58-9034-b67ccb27f317">authentication</a> and secure
exchange of information on open networks, such as the Internet, extranets, and
intranets. Certificates are digitally signed by the issuing certification
authority (CA) and can be issued for a user, a computer, or a service. The most
widely accepted format for certificates is defined by the ITU-T X.509 version 3
international standards. For more information about attributes and extensions,
see <a href="https://go.microsoft.com/fwlink/?LinkId=90414">[RFC3280]</a> and <a href="https://go.microsoft.com/fwlink/?LinkId=90590">[X509]</a> sections 7 and
8.</p>

<p><a id="gt_2df17764-8b5c-49f9-b242-08613a2ed0bb" /><b>Digest Access Authentication</b>:
A mechanism built on top of HTTP that allows a client program to provide
credentials without having to send a user name and password in plaintext when
making a request. For more information, see [RFC2617].</a></p>

<p><a id="gt_f49694cc-c350-462d-ab8e-816f0103c6c1" /><b>globally unique identifier
(GUID)</b>: A term used interchangeably with universally unique identifier
(UUID) in Microsoft protocol technical documents (TDs). Interchanging the usage
of these terms does not imply or require a specific algorithm or mechanism to
generate the value. Specifically, the use of this term does not imply or
require that the algorithms described in </a><a href="https://go.microsoft.com/fwlink/?LinkId=90460">[RFC4122]</a> or <a href="https://go.microsoft.com/fwlink/?LinkId=89824">[C706]</a> must be used
for generating the <a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_f49694cc-c350-462d-ab8e-816f0103c6c1">GUID</a>.
See also universally unique identifier (UUID).</p>

<p><a id="gt_d6a282ce-b1da-41e1-b05a-22f777a5c1fe" /><b>Kerberos</b>: An
authentication access type as defined by </a><a href="https://go.microsoft.com/fwlink/?LinkId=90304">[RFC1964]</a>.</p>

<p><a id="gt_5c2c313d-f7b8-4080-aa88-d383bc13a93a" /><b>Negotiate</b>: An
authentication access type supported by HTTP as defined by </a><a href="https://go.microsoft.com/fwlink/?LinkId=90483">[RFC4559]</a>.</p>

<p><a id="gt_fff710f9-e3d1-4991-99a2-009768d57585" /><b>NT LAN Manager (NTLM)
Authentication Protocol</b>: A protocol using a challenge-response mechanism
for </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_8e961bf0-95ba-4f58-9034-b67ccb27f317">authentication</a>
in which clients are able to verify their identities without sending a password
to the server. It consists of three messages, commonly referred to as Type 1
(negotiation), Type 2 (challenge) and Type 3 (authentication). For more
information, see <mshelp:link keywords="b38c36ed-2804-4868-a9ff-8dd3182128e4" tabindex="0">[MS-NLMP]</mshelp:link>.</p>

<p><a id="gt_17f801a6-987e-4c3e-a07c-d0acca5f3477" /><b>NWS object</b>: An instance
of the Native Web Services (NWS) protocol that is created by receiving a
sqlbatch request.</a></p>

<p><a id="gt_c1c313af-2310-4380-a6ea-c2cedc115958" /><b>SOAP</b>: A lightweight
protocol for exchanging structured information in a decentralized, distributed
environment. </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_c1c313af-2310-4380-a6ea-c2cedc115958">SOAP</a>
uses <a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_982b7f8e-d516-4fd5-8d5e-1a836081ed85">XML</a> technologies to
define an extensible messaging framework, which provides a message construct
that can be exchanged over a variety of underlying protocols. The framework has
been designed to be independent of any particular programming model and other
implementation-specific semantics. SOAP 1.2 supersedes SOAP 1.1. See <a href="https://go.microsoft.com/fwlink/?LinkId=90521">[SOAP1.2-1/2003]</a>.</p>

<p><a id="gt_c1358651-96c1-4ce0-8e1f-b0b7a94145e3" /><b>SOAP action</b>: The HTTP
request header field used to indicate the intent of the </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_c1c313af-2310-4380-a6ea-c2cedc115958">SOAP</a> request, using a URI
value. See <a href="https://go.microsoft.com/fwlink/?LinkId=90520">[SOAP1.1]</a>
section 6.1.1 for more information.</p>

<p><a id="gt_57cdf8ab-8d79-462d-a446-5d85632a7a04" /><b>SOAP body</b>: A container
for the payload data being delivered by a </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_96185df3-4677-478c-b239-f72fcf514c59">SOAP message</a> to its
recipient. See <a href="https://go.microsoft.com/fwlink/?LinkId=94664">[SOAP1.2-1/2007]</a>
section 5.3 for more information.</p>

<p><a id="gt_ec8728a8-1a75-426f-8767-aa1932c7c19f" /><b>SOAP fault</b>: A container
for error and status information within a </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_96185df3-4677-478c-b239-f72fcf514c59">SOAP message</a>. See
[SOAP1.2-1/2007] section 5.4 for more information.</p>

<p><a id="gt_093a0af2-e71c-40fc-a484-d2f802da0277" /><b>SOAP header</b>: A mechanism
for implementing extensions to a </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_96185df3-4677-478c-b239-f72fcf514c59">SOAP message</a> in a
decentralized manner without prior agreement between the communicating parties.
See [SOAP1.2-1/2007] section 5.2 for more information.</p>

<p><a id="gt_96185df3-4677-478c-b239-f72fcf514c59" /><b>SOAP message</b>: An </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_982b7f8e-d516-4fd5-8d5e-1a836081ed85">XML</a> document consisting of
a mandatory SOAP envelope, an optional <a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_093a0af2-e71c-40fc-a484-d2f802da0277">SOAP header</a>, and a
mandatory <a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_57cdf8ab-8d79-462d-a446-5d85632a7a04">SOAP body</a>. See
[SOAP1.2-1/2007] section 5 for more information.</p>

<p><a id="gt_1c1cb476-8f78-4ebd-9781-6965b3838102" /><b>SOAP mustUnderstand attribute</b>:
A global, Boolean </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_108a1419-49a9-4d19-b6ca-7206aa726b3f">attribute</a>
that is used to indicate whether a header entry is mandatory or optional for
the recipient to process. See [SOAP1.2-1/2007] section 5.2.3 for more
information.</p>

<p><a id="gt_4c9eef52-69d4-43e7-ac04-ff1fe43a94fb" /><b>UTF-16</b>: A standard for
encoding Unicode characters, defined in the Unicode standard, in which the most
commonly used characters are defined as double-byte characters. Unless
specified otherwise, this term refers to the UTF-16 encoding form specified in </a><a href="https://go.microsoft.com/fwlink/?LinkId=154659">[UNICODE5.0.0/2007]</a>
section 3.9.</p>

<p><a id="gt_409411c4-b4ed-4ab6-b0ee-6d7815f85a35" /><b>UTF-8</b>: A byte-oriented
standard for encoding Unicode characters, defined in the Unicode standard.
Unless specified otherwise, this term refers to the UTF-8 encoding form specified
in [UNICODE5.0.0/2007] section 3.9.</a></p>

<p><a id="gt_a96bfb18-c329-40f5-89fd-df7a94b89882" /><b>web service</b>: A software
system designed to support interoperable machine-to-machine interaction over a
network, using XML-based standards and open transport protocols.</a></p>

<p><a id="gt_5a824664-0858-4b09-b852-83baf4584efa" /><b>Web Services Description
Language (WSDL)</b>: An XML format for describing network services as a set of
endpoints that operate on messages that contain either document-oriented or
procedure-oriented information. The operations and messages are described
abstractly and are bound to a concrete network protocol and message format in
order to define an endpoint. Related concrete endpoints are combined into
abstract endpoints, which describe a network service. WSDL is extensible, which
allows the description of endpoints and their messages regardless of the message
formats or network protocols that are used.</a></p>

<p><a id="gt_d5ccdf11-3f53-4118-a845-dfaca61838fb" /><b>WSDL message</b>: An
abstract, typed definition of the data that is communicated during a </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_3f81265d-5456-4bfe-b795-ac5bf522b299">WSDL operation</a> <a href="https://go.microsoft.com/fwlink/?LinkId=90577">[WSDL]</a>. Also, an
element that describes the data being exchanged between web service providers
and clients.</p>

<p><a id="gt_3f81265d-5456-4bfe-b795-ac5bf522b299" /><b>WSDL operation</b>: A single
action or function of a web service. The execution of a WSDL operation
typically requires the exchange of messages between the service requestor and
the service provider.</a></p>

<p><a id="gt_61056d88-e7ee-4cea-8dcd-80a9ef5db083" /><b>WSDL port type</b>: A named
set of logically-related, abstract </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_5a824664-0858-4b09-b852-83baf4584efa">Web Services Description
Language (WSDL)</a> operations and messages.</p>

<p><a id="gt_982b7f8e-d516-4fd5-8d5e-1a836081ed85" /><b>XML</b>: The Extensible
Markup Language, as described in </a><a href="https://go.microsoft.com/fwlink/?LinkId=90599">[XML1.0]</a>.</p>

<p><a id="gt_485f05b3-df3b-45ac-b8bf-d05f5d185a24" /><b>XML namespace</b>: A
collection of names that is used to identify elements, types, and attributes in
XML documents identified in a URI reference </a><a href="https://go.microsoft.com/fwlink/?LinkId=90453">[RFC3986]</a>. A
combination of XML namespace and local name allows XML documents to use
elements, types, and attributes that have the same names but come from
different sources. For more information, see <a href="https://go.microsoft.com/fwlink/?LinkId=90602">[XMLNS-2ED]</a>.</p>

<p><a id="gt_bd0ce6f9-c350-4900-827e-951265294067" /><b>XML schema</b>: A description
of a type of XML document that is typically expressed in terms of constraints
on the structure and content of documents of that type, in addition to the
basic syntax constraints that are imposed by </a><a href="4baedaec-b5a7-4176-be88-e1cec659ab8c.html#gt_982b7f8e-d516-4fd5-8d5e-1a836081ed85">XML</a> itself. An XML schema
provides a view of a document type at a relatively high level of abstraction.</p>

<p><b>MAY,
SHOULD, MUST, SHOULD NOT, MUST NOT:</b> These terms (in all caps) are used as
defined in <a href="https://go.microsoft.com/fwlink/?LinkId=90317">[RFC2119]</a>.
All statements of optional behavior use either MAY, SHOULD, or SHOULD NOT.</p>


                </div>
            </div>
        </div>
    </body>
</html>