---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition メソッド"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "Microsoft Project が \"None\" と表示するシンプルな拡張属性定義を作成するファクトリメソッドです。"
type: docs
weight: 60
url: /ja/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Microsoft Project が \"None\" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::None に等しく、Tasks でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| customFieldType | 指定された CustomFieldType タイプです。 |
| fieldId | 指定された ExtendedAttributeTask フィールド ID。 |
| alias | 指定された System::String エイリアスです。 |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Microsoft Project が "None" と表示するシンプルな拡張属性定義を作成するファクトリメソッドです。CalculationType は Tasks::CalculationType::None に等しく、Tasks のみで使用できます。このメソッドを呼び出す際には fieldId と alias を指定する必要があります。フィールドの型はフィールド ID から推測されます。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| fieldId | 指定された ExtendedAttributeTask フィールド ID。 |
| alias | 指定された System::String エイリアスです。 |

