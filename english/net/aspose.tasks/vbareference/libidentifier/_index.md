---
title: VbaReference.LibIdentifier
second_title: Aspose.Tasks for .NET API Reference
description: VbaReference property. Gets identifier of the library
type: docs
weight: 20
url: /net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Gets identifier of the library.

```csharp
public string LibIdentifier { get; }
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


