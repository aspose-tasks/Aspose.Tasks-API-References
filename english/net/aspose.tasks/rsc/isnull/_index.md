---
title: Rsc.IsNull
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines whether a resource is null
type: docs
weight: 420
url: /net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Determines whether a resource is null.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Examples

Shows how to read/write Rsc.IsNull property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


