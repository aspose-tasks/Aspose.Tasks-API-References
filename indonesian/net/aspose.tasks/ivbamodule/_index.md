---
title: "Antarmuka IVbaModule"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Antarmuka Aspose.Tasks.IVbaModule. Mewakili modul dengan kode VBA"
type: docs
weight: 880
url: /id/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Mewakili modul dengan kode VBA.

```csharp
public interface IVbaModule
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Mendapatkan kumpulan [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Mendapatkan nama modul VBA |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Mendapatkan kode sumber dari modul VBA |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


