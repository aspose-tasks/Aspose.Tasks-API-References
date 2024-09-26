---
title: VbaReference.Name
second_title: Aspose.Tasks for .NET API Reference
description: VbaReference property. Gets or sets name of VBA reference
type: docs
weight: 30
url: /net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Gets or sets name of VBA reference.

```csharp
public string Name { get; set; }
```

## Examples

Shows how to read VBA references.

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


