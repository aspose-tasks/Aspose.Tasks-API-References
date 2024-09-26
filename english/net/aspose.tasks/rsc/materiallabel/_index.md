---
title: Rsc.MaterialLabel
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The unit of measure for the material resource
type: docs
weight: 440
url: /net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

The unit of measure for the material resource.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Examples

Shows how to read/write Rsc.MaterialLabel property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


