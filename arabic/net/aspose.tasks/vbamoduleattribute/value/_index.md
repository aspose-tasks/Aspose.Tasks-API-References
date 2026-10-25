---
title: "VbaModuleAttribute.Value"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaModuleAttribute. يحصل على قيمة سمة وحدة VBA"
type: docs
weight: 20
url: /ar/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

يحصل أو يعيّن القيمة لسمة وحدة VBA.

```csharp
public string Value { get; }
```

## الأمثلة

يظهر كيفية العمل مع سمات وحدة VBA.

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

### انظر أيضًا

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


