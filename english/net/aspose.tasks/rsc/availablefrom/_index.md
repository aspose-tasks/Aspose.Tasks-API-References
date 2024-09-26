---
title: Rsc.AvailableFrom
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The starting date that a resource is available for work at the units specified for the current time period
type: docs
weight: 120
url: /net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

The starting date that a resource is available for work at the units specified for the current time period.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Examples

Shows how to read/write Rsc.AvailableFrom property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


