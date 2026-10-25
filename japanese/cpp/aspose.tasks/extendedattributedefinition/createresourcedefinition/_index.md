---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition メソッド"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "Microsoft Project が \"None\" と表示するシンプルな拡張属性定義を作成するファクトリメソッドです。"
type: docs
weight: 50
url: /ja/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Microsoft Project が \"None\" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::None に等しく、Resource でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| customFieldType | 指定された CustomFieldType タイプです。 |
| fieldId | 指定された ExtendedAttributeResource フィールドIDです。 |
| alias | 指定された System::String エイリアスです。 |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

シンプルな拡張属性定義を作成するファクトリーメソッドで、Microsoft Project は "None" と表示します。CalculationType は Tasks::CalculationType::None に等しく、リソースでのみ使用できます。このメソッドを呼び出す際には fieldId と alias を指定する必要があります。フィールドの型は fieldId から推測されます。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| fieldId | 指定された ExtendedAttributeResource フィールドIDです。 |
| alias | 指定された System::String エイリアスです。 |

