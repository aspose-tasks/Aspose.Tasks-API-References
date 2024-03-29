---
title: Initials
second_title: Aspose.Tasks for .NET API Reference
description: The initials of a resource.
type: docs
weight: 370
url: /net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

The initials of a resource.

```csharp
public static readonly Key<string, RscKey> Initials;
```

### Examples

Shows how to read/write Rsc.Initials property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
