---
title: Rsc.MaxUnits
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The maximum number of units representing the maximum capacity for which a resource is available to accomplish any tasks during the current time period
type: docs
weight: 450
url: /net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

The maximum number of units representing the maximum capacity for which a resource is available to accomplish any tasks during the current time period.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Examples

Shows how to read/write Rsc.MaxUnits property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


