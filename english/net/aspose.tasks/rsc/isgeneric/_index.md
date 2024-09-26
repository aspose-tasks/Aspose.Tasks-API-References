---
title: Rsc.IsGeneric
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines whether a resource is generic or not
type: docs
weight: 410
url: /net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Determines whether a resource is generic or not.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Examples

Shows how to read/write Rsc.IsGeneric property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


