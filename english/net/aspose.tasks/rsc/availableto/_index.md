---
title: Rsc.AvailableTo
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The end date that a resource is available for work at the units specified for the current time period
type: docs
weight: 130
url: /net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

The end date that a resource is available for work at the units specified for the current time period.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Examples

Shows how to read/write Rsc.AvailableTo property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


