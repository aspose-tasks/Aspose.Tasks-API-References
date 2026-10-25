---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition メソッド"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "ルックアップ付きの拡張属性定義を作成するファクトリメソッドです。"
type: docs
weight: 40
url: /ja/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::Lookup に等しく、Tasks でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| customFieldType | 指定された CustomFieldType タイプです。 |
| fieldId | 指定された ExtendedAttributeTask フィールド ID。 |
| alias | 指定された System::String エイリアスです。 |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

ルックアップ付きの拡張属性定義を作成するファクトリメソッドです。CalculationType は Tasks::CalculationType::Lookup に等しく、Tasks のみで使用できます。このメソッドを呼び出す際には fieldId と alias を指定する必要があります。フィールドの型はフィールド ID から推測されます。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| fieldId | 指定された ExtendedAttributeTask フィールド ID。 |
| alias | 指定された System::String エイリアスです。 |

