---
title: "VbaModule.Name"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti VbaModule. Mendapatkan nama modul VBA"
type: docs
weight: 40
url: /id/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Mendapatkan nama modul VBA

```csharp
public string Name { get; set; }
```

## Contoh

Menampilkan cara membaca modul proyek VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Lihat Juga

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


