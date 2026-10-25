---
title: "VbaModule.Attributes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaModule. تحصل على مجموعة من سمات الوحدة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

يحصل على مجموعة من سمات الوحدة.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## الأمثلة

يظهر كيفية قراءة سمات وحدة VBA.

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

### انظر أيضًا

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


