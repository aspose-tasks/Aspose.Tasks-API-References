---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition method"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "Factory method which creates an extended attribute definition with lookup."
type: docs
weight: 40
url: /cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Tasks::CalculationType::Lookup and can be used in Tasks only. You are required to specify customFieldType , fieldId and alias when call this method.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| customFieldType | The specified CustomFieldType type. |
| fieldId | The specified ExtendedAttributeTask field ID. |
| alias | The specified System::String alias. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Tasks::CalculationType::Lookup and can be used in Tasks only. You are required to specify fieldId and alias when call this method. The field type is inferred from field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| fieldId | The specified ExtendedAttributeTask field ID. |
| alias | The specified System::String alias. |

