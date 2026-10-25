---
title: "VbaModule.Attributes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti VbaModule. Mendapatkan koleksi atribut modul"
type: docs
weight: 30
url: /id/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Mendapatkan koleksi atribut modul.

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
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


