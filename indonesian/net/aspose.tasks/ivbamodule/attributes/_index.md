---
title: "IVbaModule.Attributes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti IVbaModule. Mendapatkan koleksi VbaModuleAttributeCollection"
type: docs
weight: 10
url: /id/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Mendapatkan koleksi [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Contoh

Menunjukkan cara membaca atribut modul VBA.

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

### Lihat Juga

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


