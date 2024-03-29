---
title: Attributes
second_title: Aspose.Tasks for .NET API Reference
description: Gets a collection of VbaModuleAttributeCollectionaspose.tasks/vbamoduleattributecollection
type: docs
weight: 10
url: /net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Gets a collection of [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection)

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

### Examples

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

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection)
* interface [IVbaModule](../../ivbamodule)
* namespace [Aspose.Tasks](../../ivbamodule)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
