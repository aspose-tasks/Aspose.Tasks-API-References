---
title: "VbaModuleAttribute.Value"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "VbaModuleAttribute properti. Mendapatkan nilai atribut modul VBA"
type: docs
weight: 20
url: /id/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Mendapatkan nilai atribut modul VBA.

```csharp
public string Value { get; }
```

## Contoh

Menampilkan cara bekerja dengan atribut modul VBA.

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

### Lihat Juga

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


