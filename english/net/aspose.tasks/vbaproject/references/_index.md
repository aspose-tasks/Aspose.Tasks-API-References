---
title: VbaProject.References
second_title: Aspose.Tasks for .NET API Reference
description: VbaProject property. Gets a collection of VbaReferenceCollection
type: docs
weight: 70
url: /net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Gets a collection of [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Examples

Shows how to read VBA project reference information.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### See Also

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


