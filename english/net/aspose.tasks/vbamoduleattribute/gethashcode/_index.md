---
title: GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: Returns a hash code value for this VbaModuleAttributeaspose.tasks/vbamoduleattribute.
type: docs
weight: 40
url: /net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Returns a hash code value for this [`VbaModuleAttribute`](../../vbamoduleattribute).

```csharp
public override int GetHashCode()
```

### Return Value

Returns a hash code value for this object.

### Examples

Shows how to get a hash code of a VBA module attribute.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// print hash codes of a VBA module attributes
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### See Also

* class [VbaModuleAttribute](../../vbamoduleattribute)
* namespace [Aspose.Tasks](../../vbamoduleattribute)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
