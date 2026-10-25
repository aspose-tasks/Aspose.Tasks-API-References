---
title: "VbaModuleAttribute.Key"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti VbaModuleAttribute. Mendapatkan kunci atribut modul VBA"
type: docs
weight: 10
url: /id/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

Mendapatkan kunci atribut modul VBA.

```csharp
public string Key { get; }
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


