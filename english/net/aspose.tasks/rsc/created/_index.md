---
title: Rsc.Created
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The date and time when a resource was added to the project
type: docs
weight: 260
url: /net/aspose.tasks/rsc/created/
---
## Rsc.Created field

The date and time when a resource was added to the project.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Examples

Shows how to read/write Rsc.Created property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


