---
title: Class VbaModuleAttribute
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaModuleAttribute class. The attribute of the VbaModule object
type: docs
weight: 2740
url: /net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

The attribute of the [`VbaModule`](../vbamodule/) object

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Properties

| Name | Description |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Gets key of VBA module attribute. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Gets value of VBA module attribute. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to the specified `VbaModuleAttribute` object. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Returns a value indicating whether this instance is equal to the specified `VbaModuleAttribute` object. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Returns a hash code value for this `VbaModuleAttribute`. |

## Examples

Shows how to work with VBA module attributes.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


