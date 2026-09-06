---
title: "IVbaModule.Attributes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية IVbaModule. تحصل على مجموعة من VbaModuleAttributeCollection"
type: docs
weight: 10
url: /ar/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

تحصل على مجموعة من [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


