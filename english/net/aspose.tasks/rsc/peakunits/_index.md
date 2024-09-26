---
title: Rsc.PeakUnits
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The maximum assignment unit for a resource at any one point in time for all tasks to which the resource is assigned
type: docs
weight: 540
url: /net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

The maximum assignment unit for a resource at any one point in time for all tasks to which the resource is assigned.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Examples

Shows how to read/write Rsc.PeakUnits property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


