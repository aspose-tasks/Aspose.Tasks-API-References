---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition 方法"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 \"None\"。"
type: docs
weight: 60
url: /zh/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 CalculationType 等于 Tasks::CalculationType::None，并且只能在 Tasks 中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| customFieldType | 指定的 CustomFieldType 类型。 |
| fieldId | 指定的 ExtendedAttributeTask 字段 ID。 |
| alias | 指定的 System::String 别名。 |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 "None"。其 CalculationType 等于 Tasks::CalculationType::None，并且只能在 Tasks 中使用。调用此方法时必须指定 fieldId 和 alias。字段类型从字段 ID 推断。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| fieldId | 指定的 ExtendedAttributeTask 字段 ID。 |
| alias | 指定的 System::String 别名。 |

