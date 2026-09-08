---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ResourceAssignment メソッド。可変材料消費を伴う材料リソースの割り当てに対して単位を設定します。可変材料消費とは、割り当て期間が変わると使用される材料の量が比例して変化することを意味します。"
type: docs
weight: 760
url: /ja/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

可変材料消費を伴う材料リソースの割り当てに対して単位を設定します。可変材料消費とは、割り当て期間が変わると使用される材料の量が比例して変化することを意味します。

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 単位 | Double | 期間中に累積された単位数。 |
| rateScaleType | RateScaleType | 単位値が累積される期間。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | メソッドが非材料リソースの割り当てに対して呼び出された場合。 |

## 備考

例えば、'123/月' を設定するには、SetUnitsScaled(123D, RateScaleType.Month) を呼び出す必要があります。

## 例

材料リソースの割り当てに対して可変材料消費（例：'10/日' または '1/週'）を設定する方法を示します。

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// 例えば、'1/週' の材料消費を設定したいとします。
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### 関連項目

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


