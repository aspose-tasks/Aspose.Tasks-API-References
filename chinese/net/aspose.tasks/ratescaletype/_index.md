---
title: "枚举 RateScaleType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RateScaleType 枚举。指定费率比例类型"
type: docs
weight: 1650
url: /zh/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

指定费率比例类型。

```csharp
public enum RateScaleType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `0` | 指示未定义的费率比例类型。 |
| Minute | `1` | 指示分钟费率比例类型。 |
| Hour | `2` | 指示小时费率比例类型。 |
| Day | `3` | 指示天费率比例类型。 |
| Week | `4` | 指示周费率比例类型。 |
| Month | `5` | 指示月费率比例类型。 |
| Quarter | `6` | 指示季度费率比例类型。 |
| Year | `7` | 指示年费率比例类型。 |

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

展示在想要为材料资源的分配设置可变材料消耗（例如 '10/天' 或 '1/周'）时，如何使用分配的费率比例。

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// 假设我们想要设置 '1/周' 的材料消耗。
// 我们应该将每小时费率设置到 Units 属性，因此我们将 1D 除以每周的小时数。
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// 请注意，从 24.4 开始，可以通过调用一个方法来实现：
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// 只有材料资源分配可以拥有非零的费率比例值。
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


