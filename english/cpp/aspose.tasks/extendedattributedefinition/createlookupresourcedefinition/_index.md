---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition method"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "Factory method which creates an extended attribute definition with lookup."
type: docs
weight: 30
url: /cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Tasks::CalculationType::Lookup and can be used in Resources only. You are required to specify customFieldType , fieldId and alias when call this method.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| customFieldType | The specified CustomFieldType type. |
| fieldId | The specified ExtendedAttributeResource field ID. |
| alias | The specified System::String alias. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Tasks::CalculationType::Lookup and can be used in Resources only. You are required to specify fieldId and alias when call this method. The field type is inferred from field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| fieldId | The specified ExtendedAttributeResource field ID. |
| alias | The specified System::String alias. |

