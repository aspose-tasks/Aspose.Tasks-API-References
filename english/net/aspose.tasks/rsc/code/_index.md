---
title: Rsc.Code
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The code or other information about a resource
type: docs
weight: 210
url: /net/aspose.tasks/rsc/code/
---
## Rsc.Code field

The code or other information about a resource.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Examples

Shows how to read/write Rsc.Code property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


