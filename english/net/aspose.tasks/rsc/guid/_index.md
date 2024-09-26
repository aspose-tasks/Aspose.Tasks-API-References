---
title: Rsc.Guid
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Contains the generated unique identification code for the resource
type: docs
weight: 310
url: /net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Contains the generated unique identification code for the resource.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Examples

Shows how to read/write Rsc.Guid property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


