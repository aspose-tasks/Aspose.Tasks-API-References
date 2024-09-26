---
title: ResourceAssignment.SetMaterialResourceUnits
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Sets units for assignment of a material resource with variable material consumption. The variable material consumption means that as the assignment duration changes the quantity of materials used changes proportionally
type: docs
weight: 760
url: /net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Sets units for assignment of a material resource with variable material consumption. The variable material consumption means that as the assignment duration changes, the quantity of materials used changes proportionally.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| units | Double | Number of units accrued at the time period. |
| rateScaleType | RateScaleType | Time period at which the unit value is accrued. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If the method is called for assignment of non-material resource. |

## Remarks

For example, to set '123/month', SetUnitsScaled(123D, RateScaleType.Month) should be called.

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

### See Also

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


