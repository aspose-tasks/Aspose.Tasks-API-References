---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition メソッド"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "ルックアップ付きの拡張属性定義を作成するファクトリメソッドです。"
type: docs
weight: 30
url: /ja/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::Lookup に等しく、Resources でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| customFieldType | 指定された CustomFieldType タイプです。 |
| fieldId | 指定された ExtendedAttributeResource フィールドIDです。 |
| alias | 指定された System::String エイリアスです。 |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

ルックアップ付きの拡張属性定義を作成するファクトリメソッドです。CalculationType は Tasks::CalculationType::Lookup に等しく、Resources のみで使用できます。このメソッドを呼び出す際には fieldId と alias を指定する必要があります。フィールドの型はフィールド ID から推測されます。

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| パラメーター | 説明 |
| --- | --- |
| fieldId | 指定された ExtendedAttributeResource フィールドIDです。 |
| alias | 指定された System::String エイリアスです。 |

