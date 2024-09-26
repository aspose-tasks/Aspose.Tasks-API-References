---
title: Asn.PercentWorkComplete
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The amount of a work completed on an assignment
type: docs
weight: 400
url: /net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

The amount of a work completed on an assignment.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Examples

Shows how to read percent work complete of an assignment.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Print assignment percent completion
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


