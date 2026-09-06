---
title: "Asn.RateScale"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。材料资源分配使用率的时间单位。如果未定义则返回 0"
type: docs
weight: 410
url: /zh/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

物料资源分配的使用率的时间单位。如果未定义，则返回 0。

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## 示例

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


