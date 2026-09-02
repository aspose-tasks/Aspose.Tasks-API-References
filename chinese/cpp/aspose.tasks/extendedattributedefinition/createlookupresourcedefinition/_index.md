---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition 方法"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "工厂方法，用于创建带有查找的扩展属性定义。"
type: docs
weight: 30
url: /zh/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

工厂方法，用于创建带查找的扩展属性定义。其 CalculationType 等于 Tasks::CalculationType::Lookup，并且只能在 Resources 中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| customFieldType | 指定的 CustomFieldType 类型。 |
| fieldId | 指定的 ExtendedAttributeResource 字段 ID。 |
| alias | 指定的 System::String 别名。 |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

工厂方法用于创建带查找的扩展属性定义。其 CalculationType 等于 Tasks::CalculationType::Lookup，并且只能在 Resources 中使用。调用此方法时必须指定 fieldId 和 alias。字段类型从字段 ID 推断。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| fieldId | 指定的 ExtendedAttributeResource 字段 ID。 |
| alias | 指定的 System::String 别名。 |

