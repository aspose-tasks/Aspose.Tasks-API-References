---
title: Rsc.IsEnterprise
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Shows whether a resource is from the enterprise resource pool true or the local resource pool false
type: docs
weight: 400
url: /net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Shows whether a resource is from the enterprise resource pool (true) or the local resource pool (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Examples

Shows how to read/write Rsc.IsEnterprise property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


