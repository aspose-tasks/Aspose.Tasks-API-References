---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition method"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "Factory method which creates a simple extended attribute definition, which Microsoft Project shows as \"None\"."
type: docs
weight: 50
url: /cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has CalculationType equals to Tasks::CalculationType::None and can be used in Resource only. You are required to specify customFieldType , fieldId and alias when call this method.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| customFieldType | The specified CustomFieldType type. |
| fieldId | The specified ExtendedAttributeResource field ID. |
| alias | The specified System::String alias. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has CalculationType equals to Tasks::CalculationType::None and can be used in Resource only. You are required to specify fieldId and alias when call this method. The field type is inferred from field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| fieldId | The specified ExtendedAttributeResource field ID. |
| alias | The specified System::String alias. |

