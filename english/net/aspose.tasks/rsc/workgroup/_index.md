---
title: Rsc.Workgroup
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The type of a workgroup to which a resource belongs
type: docs
weight: 700
url: /net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

The type of a workgroup to which a resource belongs.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Examples

Shows how to read/write Rsc.Workgroup property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


