---
title: VbaModule.Attributes
second_title: Aspose.Tasks for .NET API Reference
description: VbaModule property. Gets a collection of the modules attributes
type: docs
weight: 30
url: /net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Gets a collection of the module's attributes.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Examples

Shows how to read VBA module's attributes.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### See Also

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


