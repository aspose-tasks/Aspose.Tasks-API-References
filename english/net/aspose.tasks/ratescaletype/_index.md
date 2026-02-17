---
title: Enum RateScaleType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RateScaleType enum. Specifies the rate scale type
type: docs
weight: 1630
url: /net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Specifies the rate scale type.

```csharp
public enum RateScaleType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `0` | Indicates Undefined rate scale type. |
| Minute | `1` | Indicates Minute rate scale type. |
| Hour | `2` | Indicates Hour rate scale type. |
| Day | `3` | Indicates Day rate scale type. |
| Week | `4` | Indicates Week rate scale type. |
| Month | `5` | Indicates Month rate scale type. |
| Quarter | `6` | Indicates Quarter rate scale type. |
| Year | `7` | Indicates Year rate scale type. |

## Examples

Shows how to set variable material consumption (e.g. '10/day' or '1/week') for an assignment of a material resource.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Suppose we want to set '1/week' material consumption.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

Shows how to work with assignment's rate scale when we want to set variable material consumption (e.g. '10/day' or '1/week') for an assignment of a material resource.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Suppose we want to set '1/week' material consumption.
// We should set hourly rate to Units property, so we divide 1D by hours per week.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Please note that starting with 24.4. this can be done by calling 1 method:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// only material resource assignments can have non-zero rate scale value.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


