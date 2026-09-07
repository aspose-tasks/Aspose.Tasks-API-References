---
title: "Kelas VbaModule"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.VbaModule. Mewakili modul VBA"
type: docs
weight: 2810
url: /id/net/aspose.tasks/vbamodule/
---
## VbaModule class

Mewakili modul VBA.

```csharp
public sealed class VbaModule
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Mendapatkan koleksi atribut modul. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Mendapatkan nama modul VBA |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Mendapatkan atau mengatur kode sumber modul VBA |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Mendapatkan tipe modul. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Membuat instance `VbaModule` dengan tipe VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Membuat instance `VbaModule` dengan tipe VbaModuleType.ProceduralModule. |

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


