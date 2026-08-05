---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition method"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "Factory method which creates a simple extended attribute definition, which Microsoft Project shows as \"None\"."
type: docs
weight: 60
url: /cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has CalculationType equals to Tasks::CalculationType::None and can be used in Tasks only. You are required to specify customFieldType , fieldId and alias when calling this method.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| customFieldType | The specified CustomFieldType type. |
| fieldId | The specified ExtendedAttributeTask field ID. |
| alias | The specified System::String alias. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has CalculationType equals to Tasks::CalculationType::None and can be used in Tasks only. You are required to specify fieldId and alias when calling this method. The field type is inferred from field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Description |
| --- | --- |
| fieldId | The specified ExtendedAttributeTask field ID. |
| alias | The specified System::String alias. |

