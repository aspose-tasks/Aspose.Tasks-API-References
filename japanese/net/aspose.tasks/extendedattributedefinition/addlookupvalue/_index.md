---
title: AddLookupValue
second_title: Aspose.Tasks for .NET API リファレンス
description: 内部参照リストに値を追加しますこれはValueListaspose.tasks/extendedattributedefinition/valuelist/.
type: docs
weight: 290
url: /ja/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

内部参照リストに値を追加します。これは、[`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| value | Value | ルックアップに追加する値。 |

### 備考

このメソッドは、[`ExtendedAttributeDefinition`](../)持っているinstances [`CalculationType`](../calculationtype/)に等しいLookup.

### 例

このコードを使用して、ルックアップ リストに新しい値を追加します:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### 関連項目

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* 名前空間 [Aspose.Tasks](../../extendedattributedefinition/)
* 組み立て [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
