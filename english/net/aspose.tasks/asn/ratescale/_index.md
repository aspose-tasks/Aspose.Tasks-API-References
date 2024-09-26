---
title: Asn.RateScale
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The time unit for the usage rate of the material resource assignment. Returns 0 if not defined
type: docs
weight: 410
url: /net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

The time unit for the usage rate of the material resource assignment. Returns 0 if not defined.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Examples

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


