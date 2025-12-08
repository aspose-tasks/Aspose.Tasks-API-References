---
title: Class VbaReference
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaReference class. Represents a reference of the VbaProject
type: docs
weight: 2820
url: /net/aspose.tasks/vbareference/
---
## VbaReference class

Represents a reference of the [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Constructors

| Name | Description |
| --- | --- |
| [VbaReference](vbareference/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Gets identifier of the library. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Gets or sets name of VBA reference. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to the specified `VbaReference` object. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Returns a value indicating whether this instance is equal to the specified `VbaReference` object. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Returns a hash code value for this `VbaReference`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


