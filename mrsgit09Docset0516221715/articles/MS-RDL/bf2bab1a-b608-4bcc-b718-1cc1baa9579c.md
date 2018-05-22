<html dir="LTR" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:tool="http://www.microsoft.com/tooltip">
    <head>
        <meta http-equiv="Content-Type" content="text/html; CHARSET=utf-8"></meta>
        <meta name="save" content="history"></meta>
        <title>5.5 RDL XML Schema for Version 2011/01</title>
        <xml>
            <mshelp:toctitle title="5.5 RDL XML Schema for Version 2011/01"></mshelp:toctitle>
            <mshelp:rltitle title="[MS-RDL]: RDL XML Schema for Version 2011/01"></mshelp:rltitle>
            <mshelp:keyword index="A" term="bf2bab1a-b608-4bcc-b718-1cc1baa9579c"></mshelp:keyword>
            <mshelp:attr name="DCSext.ContentType" value="open specification"></mshelp:attr>
            <mshelp:attr name="AssetID" value="bf2bab1a-b608-4bcc-b718-1cc1baa9579c"></mshelp:attr>
            <mshelp:attr name="TopicType" value="kbRef"></mshelp:attr>
            <mshelp:attr name="DCSext.Title" value="[MS-RDL]: RDL XML Schema for Version 2011/01" />
        </xml>
    </head>
    <body>
        <div id="header">
            <h1 class="heading">5.5 RDL XML Schema for Version 2011/01</h1>
        </div>
        <div id="mainSection">
            <div id="mainBody">
                <div id="allHistory" class="saveHistory"></div>
                <div id="sectionSection0" class="section" name="collapseableSection">
                    

<p><b>Note:</b> RDL 2011/01 is not a complete schema. It is a
micro-versioned schema and uses <a href="3428e690-a348-4ec7-8a6a-8efb42d2cdee.htm">RDL 2010/01</a> as its base
schema. For more information about macro- and micro-versioned RDL schemas, see
section <a href="ae14822f-9553-45f1-bacc-c0a1cbb484fb.htm">2.1</a>.</p>

<dl>
<dd>
<div><pre> &lt;?xml version=&quot;1.0&quot; encoding=&quot;utf-8&quot;?&gt;
 &lt;xsd:schema targetNamespace=&quot;http://schemas.microsoft.com/sqlserver/reporting/2011/01/reportdefinition&quot; 
             xmlns:xsd=&quot;http://www.w3.org/2001/XMLSchema&quot; 
             xmlns=&quot;http://schemas.microsoft.com/sqlserver/reporting/2011/01/reportdefinition&quot; 
             xmlns:rdl2010=&quot;http://schemas.microsoft.com/sqlserver/reporting/2010/01/reportdefinition&quot;
             elementFormDefault=&quot;qualified&quot;&gt;
   &lt;xsd:annotation&gt;
     &lt;xsd:documentation&gt;
  
       The following schema describes the structure of the
       Report Definition Language (RDL) for Microsoft SQL Server 2008 R2.
  
       THE SCHEMA IS PROVIDED TO YOU ON AN &quot;AS IS&quot; BASIS, AND MICROSOFT
       DISCLAIMS ALL WARRANTIES, EXPRESS, IMPLIED OR STATUTORY,   INCLUDING,
       WITHOUT LIMITATION, THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS
       FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT, AS TO THE SCHEMA OR ANY
       PRODUCT OR OTHER ITEM THAT MAY BE DEVELOPED USING THE SCHEMA.
  
       Without limiting the generality of the foregoing, Microsoft makes no
       warranty that any product or other item that may be developed using the
       schema, or any portion of the schema, will not infringe any copyright,
       patent, trade secret or other intellectual property right of any
       individual or legal entity in any country. It is your responsibility to
       obtain licenses to use any such intellectual property rights as appropriate.
  
       MICROSOFT IS NOT LIABLE FOR ANY DAMAGES OF ANY KIND ARISING OUT OF OR IN
       CONNECTION WITH THE USE OF THE SCHEMA, INCLUDING, WITHOUT LIMITATION, ANY
       DIRECT, INDIRECT, INCIDENTAL, CONSEQUENTIAL (INCLUDING LOST REVENUES OR LOST
       PROFITS), PUNITIVE OR SPECIAL DAMAGES, WHETHER OR NOT MICROSOFT HAS BEEN
       ADVISED OF SUCH DAMAGES.
  
       (c) Microsoft Corporation.  All rights reserved.
  
     &lt;/xsd:documentation&gt;
   &lt;/xsd:annotation&gt;
  
   &lt;xsd:import namespace=&quot;http://schemas.microsoft.com/sqlserver/reporting/2010/01/reportdefinition&quot;/&gt;
   
   &lt;!--The following element is an RDL property that indicates if a Tablix is scrollable. 
   Needs to be added under the Tablix element --&gt;
   &lt;xsd:element name =&quot;CanScroll&quot; type=&quot;xsd:boolean&quot; /&gt;
   
   &lt;!--The following element is an RDL property that indicates if a Textbox is vertically scrollable. 
   Needs to be added under the Textbox element --&gt;
   &lt;xsd:element name =&quot;CanScrollVertically&quot; type=&quot;xsd:boolean&quot; /&gt;
  
   &lt;!-- May be placed on an Group to indicate the data is pre-grouped
   by the query --&gt;
   &lt;xsd:element name=&quot;NaturalGroup&quot; type=&quot;xsd:boolean&quot; /&gt;
  
   &lt;!--The following element is an RDL property that defines the dataset to use for this scope. 
   Needs to be added under the following elements: Group, TablixCell, ChartDataPoint, DataValue --&gt;
   &lt;xsd:element name =&quot;DataSetName&quot; type=&quot;xsd:string&quot; /&gt;
  
   &lt;!--The following element is an RDL property that defines the relationship to use for 
   correlating data in the parent scope with the data in the containing scope. 
   Needs to be added under the following elements: DataRegion, Group --&gt;
   &lt;xsd:element name =&quot;Relationship&quot; type=&quot;RelationshipType&quot; /&gt;
  
   &lt;!--The following element is an RDL property that defines the relationship to use for 
   correlating data in the parent scope with the data in the containing scope. 
   Needs to be added under the following elements: TablixCell, ChartDataPoint, DataValue --&gt;
   &lt;xsd:element name =&quot;Relationships&quot; type=&quot;RelationshipsType&quot; /&gt;
  
   &lt;!--The following element is an RDL property that represents default relationships to use between 
   the containing data set and other data sets when nested scopes use different data sets. 
   Needs to be added under the DataSet element --&gt;
   &lt;xsd:element name =&quot;DefaultRelationships&quot; type=&quot;DefaultRelationshipsType&quot; /&gt;
  
   &lt;xsd:complexType name=&quot;RelationshipsType&quot;&gt;
     &lt;xsd:sequence&gt;
       &lt;xsd:element name=&quot;Relationship&quot; type=&quot;RelationshipType&quot; minOccurs=&quot;1&quot;  
                    maxOccurs=&quot;unbounded&quot; /&gt;
     &lt;/xsd:sequence&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;RelationshipType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;ParentScope&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;NaturalJoin&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;JoinConditions&quot; type=&quot;JoinConditionsType&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;JoinConditionsType&quot;&gt;
     &lt;xsd:sequence&gt;
       &lt;xsd:element name=&quot;JoinCondition&quot; type=&quot;JoinConditionType&quot; minOccurs=&quot;1&quot; 
                    maxOccurs=&quot;unbounded&quot; /&gt;
     &lt;/xsd:sequence&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;JoinConditionType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;ForeignKey&quot; type=&quot;xsd:string&quot; /&gt;
       &lt;xsd:element name=&quot;PrimaryKey&quot; type=&quot;xsd:string&quot; /&gt;
       &lt;xsd:element name=&quot;SortDirection&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
         &lt;xsd:simpleType&gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
             &lt;xsd:enumeration value=&quot;Ascending&quot;/&gt;
             &lt;xsd:enumeration value=&quot;Descending&quot;/&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;DefaultRelationshipsType&quot;&gt;
     &lt;xsd:sequence&gt;
       &lt;xsd:element name=&quot;DefaultRelationship&quot; type=&quot;DefaultRelationshipType&quot; minOccurs=&quot;1&quot; 
                    maxOccurs=&quot;unbounded&quot; /&gt;
     &lt;/xsd:sequence&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;DefaultRelationshipType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;RelatedDataSet&quot; type=&quot;xsd:string&quot; /&gt;
       &lt;xsd:element name=&quot;NaturalJoin&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:element name=&quot;JoinConditions&quot; type=&quot;JoinConditionsType&quot; minOccurs=&quot;0&quot; /&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
  
   &lt;!-- May be placed on a SortExpression element to indicate the data is pre-sorted
   by the query and that sort condition --&gt;
   &lt;xsd:element name=&quot;NaturalSort&quot; type=&quot;xsd:boolean&quot; /&gt;
  
 &lt;!-- May be placed on a SortExpression element to indicate the sort should be deferred. --&gt;
   &lt;xsd:element name=&quot;DeferredSort&quot; type=&quot;xsd:boolean&quot; /&gt;
   
   &lt;!--The following element is an RDL property to represent a Tablix as a Band. 
   Needs to be added under the Tablix element --&gt;
   &lt;xsd:element name =&quot;BandLayoutOptions&quot;&gt;
     &lt;xsd:complexType&gt;
       &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
         &lt;xsd:element name=&quot;RowCount&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
           &lt;xsd:simpleType&gt;
             &lt;xsd:restriction base=&quot;xsd:unsignedInt&quot;&gt;
               &lt;xsd:minInclusive value=&quot;1&quot;/&gt;
             &lt;/xsd:restriction&gt;
           &lt;/xsd:simpleType&gt;
         &lt;/xsd:element&gt;
         &lt;xsd:element name=&quot;ColumnCount&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
           &lt;xsd:simpleType&gt;
             &lt;xsd:restriction base=&quot;xsd:unsignedInt&quot;&gt;
               &lt;xsd:minInclusive value=&quot;1&quot;/&gt;
             &lt;/xsd:restriction&gt;
           &lt;/xsd:simpleType&gt;
         &lt;/xsd:element&gt;
         &lt;xsd:element name=&quot;Coverflow&quot; type=&quot;CoverflowType&quot; minOccurs=&quot;0&quot;/&gt;
         &lt;xsd:element name=&quot;PlayAxis&quot; type=&quot;PlayAxisType&quot; minOccurs=&quot;0&quot;/&gt;
         &lt;xsd:element name=&quot;Tabstrip&quot; type=&quot;TabstripType&quot; minOccurs=&quot;0&quot;/&gt;
         &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
       &lt;/xsd:choice&gt;
       &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:complexType&gt;
   &lt;/xsd:element&gt;
   
   &lt;xsd:complexType name=&quot;NavigationItemType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;ReportItemReference&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;  
                    maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;ReportItem&quot; type=&quot;rdl2010:ReportItemsType&quot; minOccurs=&quot;0&quot;  
                    maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
   
   &lt;xsd:complexType name=&quot;CoverflowType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;NavigationItem&quot; type=&quot;NavigationItemType&quot; minOccurs=&quot;0&quot;  
                    maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;Slider&quot; type=&quot;SliderType&quot; minOccurs=&quot;0&quot;  maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;TabstripType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;NavigationItem&quot; type=&quot;NavigationItemType&quot; minOccurs=&quot;0&quot;  
                    maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;Slider&quot; type=&quot;SliderType&quot; minOccurs=&quot;0&quot;  maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;xsd:complexType name=&quot;PlayAxisType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;Slider&quot; type=&quot;SliderType&quot; minOccurs=&quot;0&quot;  maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;DockingOption&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;&gt;
         &lt;xsd:simpleType&gt;
           &lt;xsd:restriction base=&quot;xsd:string&quot;&gt;
             &lt;xsd:enumeration value=&quot;Top&quot;/&gt;
             &lt;xsd:enumeration value=&quot;Bottom&quot;/&gt;
           &lt;/xsd:restriction&gt;
         &lt;/xsd:simpleType&gt;
       &lt;/xsd:element&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
   
   &lt;xsd:complexType name=&quot;SliderType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;Hidden&quot; type=&quot;xsd:boolean&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;LabelData&quot; type=&quot;LabelDataType&quot; minOccurs=&quot;0&quot;  maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
   
   &lt;xsd:complexType name=&quot;LabelDataType&quot;&gt;
     &lt;xsd:choice minOccurs=&quot;1&quot; maxOccurs=&quot;unbounded&quot;&gt;
       &lt;xsd:element name=&quot;DataSetName&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;Key&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;  maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:element name=&quot;Label&quot; type=&quot;xsd:string&quot; minOccurs=&quot;0&quot;  maxOccurs=&quot;1&quot;/&gt;
       &lt;xsd:any namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
     &lt;/xsd:choice&gt;
     &lt;xsd:anyAttribute namespace=&quot;##other&quot; processContents=&quot;lax&quot; /&gt;
   &lt;/xsd:complexType&gt;
  
   &lt;!--The following elements are RDL properties to represent navigation UI for banding.
   Needs to be added under the Tablix element --&gt;
   &lt;xsd:element name=&quot;LeftMargin&quot; type=&quot;xsd:string&quot; /&gt;
   &lt;xsd:element name=&quot;RightMargin&quot; type=&quot;xsd:string&quot; /&gt;
   &lt;xsd:element name=&quot;TopMargin&quot; type=&quot;xsd:string&quot; /&gt;
   &lt;xsd:element name=&quot;BottomMargin&quot; type=&quot;xsd:string&quot; /&gt;
  
   &lt;!-- Add the following under the ChartDataPointValuesType.  This is for Chart Highlighting --&gt;
   &lt;xsd:element name=&quot;HighlightX&quot; type=&quot;xsd:string&quot; /&gt;
   &lt;xsd:element name=&quot;HighlightY&quot; type=&quot;xsd:string&quot; /&gt;
   &lt;xsd:element name=&quot;HighlightSize&quot; type=&quot;xsd:string&quot; /&gt;
  
   &lt;!--The following element is an RDL property that defines how to interpret subtotal data in queries. 
   May be under the RDL Field element --&gt;
   &lt;xsd:element name =&quot;AggregateIndicatorField&quot; type=&quot;xsd:string&quot; /&gt;
  
   &lt;!--The following element is an RDL property that defines how nulls should be sorted. 
   May be under the RDL DataSet element --&gt;
   &lt;xsd:element name =&quot;NullsAsBlanks&quot; type=&quot;xsd:boolean&quot; /&gt;
  
   &lt;!--The following element is an RDL property that defines the culture name to use for collation information.
   May be under the RDL DataSet element --&gt;
   &lt;xsd:element name =&quot;CollationCulture&quot; type=&quot;xsd:string&quot; /&gt;
  
 &lt;!--The following element is an RDL property that defines extra information, such as the key of a database image used for async retrieval.
   May be under the RDL Image element --&gt;
   &lt;xsd:element name =&quot;Tag&quot; type=&quot;xsd:string&quot; /&gt;
  
 &lt;!--The following attribute is an RDL property that defines a unqiue name.
   May be under the RDL ReportSection element --&gt;
   &lt;xsd:attribute name=&quot;Name&quot; type=&quot;xsd:string&quot; /&gt;
  
 &lt;/xsd:schema&gt;
</pre></div>
</dd></dl>


                </div>
            </div>
        </div>
    </body>
</html>