---
title: Rsc.CanLevel
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines whether resource leveling can be done on a resource
type: docs
weight: 200
url: /net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Determines whether resource leveling can be done on a resource.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Examples

Shows how to read/write Rsc.CanLevel property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


