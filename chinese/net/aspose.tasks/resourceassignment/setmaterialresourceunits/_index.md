---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。为具有可变材料消耗的材料资源分配设置单位。可变材料消耗意味着随着分配持续时间的变化，使用的材料数量按比例变化。"
type: docs
weight: 760
url: /zh/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

为具有可变材料消耗的材料资源分配设置单位。可变材料消耗意味着随着分配持续时间的变化，使用的材料数量按比例变化。

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 单位 | Double | 在该时间段累计的单位数量。 |
| rateScaleType | RateScaleType | 累计单位值的时间段。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果该方法用于非材料资源的分配。 |

## 备注

例如，要设置 '123/月'，应调用 SetUnitsScaled(123D, RateScaleType.Month)。

## 示例

展示如何为材料资源的分配设置可变材料消耗（例如 '10/天' 或 '1/周'）。

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// 假设我们想要设置 '1/周' 的材料消耗。
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### 另见

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


