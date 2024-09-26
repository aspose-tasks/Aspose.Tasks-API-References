---
title: Rsc.Type
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The type of a resource
type: docs
weight: 660
url: /net/aspose.tasks/rsc/type/
---
## Rsc.Type field

The type of a resource.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Examples

Shows how to read/write Rsc.Type property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


