---
title: VbaModuleAttribute.Value
second_title: Aspose.Tasks for .NET API Reference
description: VbaModuleAttribute property. Gets value of VBA module attribute
type: docs
weight: 20
url: /net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Gets value of VBA module attribute.

```csharp
public string Value { get; }
```

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

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


