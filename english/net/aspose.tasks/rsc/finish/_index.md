---
title: Rsc.Finish
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The date when a resource is scheduled to complete work on all assigned tasks
type: docs
weight: 290
url: /net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

The date when a resource is scheduled to complete work on all assigned tasks.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Examples

Shows how to read/write Rsc.Finish property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


