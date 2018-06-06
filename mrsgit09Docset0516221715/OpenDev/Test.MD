# Interoperability Test Tools

Microsoft offers the following interoperability testing opportunities and support to assist developers who are implementing the Microsoft Open Specifications:

* Microsoft Message Analyzer
* Microsoft Protocol Test Suites
* OData Validator
* Plugfests and events
* Interoperability labs
* Microsoft Office Binary File
* Format Validator
* Microsoft Exchange RPC Extractor

If you have questions about these opportunities or are interested in additional interoperability tests and tools, the [Interoperability Test Team]("mailto:interoptesttools@microsoft.com") is available to work with you to identify those tests and tools that will meet your specific needs.

## Microsoft Message Analyzer

---
Developers can use this tool in conjunction with relevant Open Specifications to further understand how Microsoft products communicate with each other. Message Analyzer exposes validation problems and behaviors so that developers can find issues with their implementations. Automatic message reassembly and diagnosis are two features that make Message Analyzer a superior tool when you are trying to access protocol compatibility. Also, built-in parser updates ensure that you have the most current protocol parsers.

You can get information and details from the [download page]("https://www.microsoft.com/en-us/download/details.aspx?id=44226").

For support, please visit the [Message Analyzer blog]("http://blogs.technet.com/b/messageanalyzer/"), or for specific questions, use the [Message Analyzer forums]("http://social.technet.microsoft.com/forums/en-us/home?forum=messageanalyzer"). For guidance information, see the Microsoft [Message Analyzer Operating Guide documentation on TechNet]("https://technet.microsoft.com/en-us/library/jj649776.aspx").

## Microsoft Protocol Test Suites

---
Originally developed for in-house testing of the Microsoft Open Specifications, the Microsoft Protocol Test Suites (Test Suites) have been used extensively during Plugfests and interoperability labs to test partner implementations. They evaluate whether a protocol implementation meets certain interoperability requirements. Test Suites do not cover every protocol requirement and in no way certify an implementation, even if all tests pass. However, each Test Suite provides users with a useful indication of interoperability. In addition, the Test Suites can be extended and integrated, because we've included the source code.

The following Microsoft Protocol Test Suites are available on GitHub and may be used by anyone (for details, see the end user license agreement for each Test Suite). Both require the [Protocol Test Framework (PTF)]("https://github.com/microsoft/protocoltestframework").

* [Office Protocol Test Suites for Office, SharePoint, and Exchange]("https://github.com/OfficeDev/Interop-TestSuites")
* [Windows Protocol Test Suites]("https://github.com/Microsoft/WindowsProtocolTestSuites")

## OData Validator

---
As a key part of the ecosystem surrounding the OData protocol, the [OData Validator]("http://services.odata.org/validation/") serves as a tool to validate OData server responses. Each rule extracted from the OData specification is a direct interpretation of a requirement as defined in the OData protocol specification. Implementers can point the tool to an endpoint and select what needs to be validated. The tool executes the right set of rules against the payload and returns a pass or fail result set. The tool supports validating various OData payloads like service document, metadata document, feed, entity and error payloads.

## Plugfests and Events

---
Microsoft offers developers the opportunity to learn more about specific protocols and to test their implementations of those protocols at these Microsoft-campus group events. [Plugfests]("https://msdn.microsoft.com/openspecifications/dn750988") include one-on-one discussions with Microsoft engineers and the use of protocol test suites that help evaluate whether an implementation's protocol communications conform to the relevant Microsoft Open Specifications. File format events offer tools to verify the interoperability of file format implementations.

## Interoperability Labs

---
Microsoft offers interoperability labs for Open Specifications developers who are facing unique technical issues. Interoperability lab participants engage in focused one-on-one testing sessions in the [Microsoft Enterprise Engineering Center]("https://www.microsoft.com/en-us/server-cloud/products/windows-server-2012-r2/default.aspx"), a world-class interoperability lab on the Redmond campus.  This highly-customized interaction allows attendees to dive deeply into their implementations by taking advantage of the latest and best hardware and extensive access to Microsoft engineers to build and run test cases in a variety of different scenarios to validate their implementations and quickly work through any issues.

Testing in this facility requires extensive setup and resources, and therefore customer-specific interoperability labs are scheduled based on lab availability.  Space is limited and priority will be given to companies who hold licenses through one of the [Microsoft Open Specifications programs]("https://msdn.microsoft.com/openspecifications/dn646761").

For more details about working with Microsoft engineers at an interoperability lab, please contact the [Interoperability Test Team]("mailto:interoptesttools@microsoft.com").

## Microsoft Office Binary File Format Validator

---
The Microsoft Office Binary File Format Validator (BBFValidator) Beta tool validates .doc, .xls and .ppt binary file format conformance to the [binary file format Open Specifications]("https://msdn.microsoft.com/en-us/library/cc313105(office.12).aspx"). This command-line tools runs without requiring an installation of Word, Excel or PowerPoint on the computer.

## Microsoft Exchange RPC Extractor

---
Microsoft Exchange RPC Extractor (RPX) is a command-line tool that can parse network captures and interpret remote procedure calls made from a client to Microsoft Exchange. RPX uses the information provided in the Microsoft Exchange protocol documentation to parse RPCs, remote operations (ROPs), and the parameters for each ROP.
