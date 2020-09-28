---
name: Data Model Change
about: Issue template to suggest a change to the data model
title: ''
labels: ''
assignees: ''

---

## **Description**
\<description\>

### **New Classes**

Package | Class | Parent Class | Description | Service
----- | ----- | ----- | ----- | -----
IEC619##\<package\>:<sub_package> | <class_name> | <parent_class_name> | <class_description> | <service_responsible_for_class>

### **New Attributes**

####  **<class_name>**
Attribute | Type | Description
----- | ----- | -----
<attribute_name> | <attribute_type> | <attribute_description>

### New Enumerations
Package | Enumeration | Description
----- | ----- | -----
IEC619##:\<package\>:<sub_package> | <enum_name> | <enum_description>

### New Enumeration Values
#### <enumeration_name>
Package: <package_name>

Value | Description
----- | ----- |
\<value\> | <enum_value_description>

### New Relationships
Source Class | Name | Target Class | Mult. | Description | Implementation Type
----- | ----- | ----- | ----- | ----- | -----
<source_class> | \<name\> | <target_class> | \<multiplicity\> | <directional_description> |  [ Direct / MRID Index - Direct = The association exists in code. MRID Index = The MRID of the Target is stored only. ] 

### New Index
_An index represents a way of querying data to retrieve a specific relationship. For example, DiagramService provides_ {{getDiagramObject(mRID: String)}} _to retrieve the DiagramObjects for a given IdentifiedObject._

Class | Function Signature | Implemented Relationship
----- | ----- | ----- |
<service_class_name, e.g Network Service> | <function_name, (param1, …)> | IdentifiedObject → DiagramObject 


- [ ] Is this an issue with impediment
