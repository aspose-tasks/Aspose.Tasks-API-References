---
title: Rsc.Name
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The name of a resource
type: docs
weight: 460
url: /net/aspose.tasks/rsc/name/
---
## Rsc.Name field

The name of a resource.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Examples

Shows how to read/write Rsc.Name property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


