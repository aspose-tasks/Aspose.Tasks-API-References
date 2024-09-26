---
title: Rsc.Inactive
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines whether a resource was made inactive by a user who has administrative rights
type: docs
weight: 360
url: /net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Determines whether a resource was made inactive by a user who has administrative rights.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Examples

Shows how to read/write Rsc.Inactive property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


