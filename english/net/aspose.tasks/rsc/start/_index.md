---
title: Rsc.Start
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The date when an assigned resource is scheduled to begin working on a task
type: docs
weight: 640
url: /net/aspose.tasks/rsc/start/
---
## Rsc.Start field

The date when an assigned resource is scheduled to begin working on a task.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Examples

Shows how to read/write Rsc.Start property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


