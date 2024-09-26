---
title: Rsc.StandardRate
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The rate of pay for regular nonovertime work performed by a resource
type: docs
weight: 620
url: /net/aspose.tasks/rsc/standardrate/
---
## Rsc.StandardRate field

The rate of pay for regular, non-overtime work performed by a resource.

```csharp
public static readonly Key<decimal, RscKey> StandardRate;
```

## Examples

Shows how to work resources rates and groups.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Add resource and set some properties
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


