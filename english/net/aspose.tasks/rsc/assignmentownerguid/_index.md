---
title: Rsc.AssignmentOwnerGuid
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The GUID of an assignment owner
type: docs
weight: 110
url: /net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

The GUID of an assignment owner.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Examples

Shows how to read/write Rsc.AssignmentOwnerGuid property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


