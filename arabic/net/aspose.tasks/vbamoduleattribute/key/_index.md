---
title: "VbaModuleAttribute.Key"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaModuleAttribute. يحصل على مفتاح سمة وحدة VBA"
type: docs
weight: 10
url: /ar/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

يحصل أو يعيّن المفتاح لسمة وحدة VBA.

```csharp
public string Key { get; }
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


