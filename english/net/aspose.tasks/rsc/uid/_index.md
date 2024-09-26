---
title: Rsc.Uid
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The unique identifier of a resource
type: docs
weight: 670
url: /net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

The unique identifier of a resource.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Examples

Shows how to read/write Rsc.Uid property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


