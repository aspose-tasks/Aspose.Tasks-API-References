---
title: Rsc.Id
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The position identifier of a resource within the list of resources
type: docs
weight: 350
url: /net/aspose.tasks/rsc/id/
---
## Rsc.Id field

The position identifier of a resource within the list of resources.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Examples

Shows how to read/write Rsc.Id property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


