---
title: Rsc.IsBudget
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines whether a work material or cost resource is a budget resource
type: docs
weight: 380
url: /net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Determines whether a work, material, or cost resource is a budget resource.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Examples

Shows how to read/write Rsc.IsBudget property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


