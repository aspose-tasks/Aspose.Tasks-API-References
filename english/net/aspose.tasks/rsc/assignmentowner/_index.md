---
title: AssignmentOwner
second_title: Aspose.Tasks for .NET API Reference
description: The name of an assignment owner.
type: docs
weight: 100
url: /net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

The name of an assignment owner.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

### Examples

Shows how to read/write Rsc.AssignmentOwner property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
