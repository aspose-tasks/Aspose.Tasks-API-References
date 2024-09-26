---
title: Rsc.IsCostResource
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines whether a resource is a cost resource
type: docs
weight: 390
url: /net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Determines whether a resource is a cost resource.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Examples

Shows how to read/write Rsc.IsCostResource property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


