---
title: "IVbaModule.SourceCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti IVbaModule. Mendapatkan kode sumber modul VBA"
type: docs
weight: 30
url: /id/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Mendapatkan kode sumber dari modul VBA

```csharp
public string SourceCode { get; }
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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


