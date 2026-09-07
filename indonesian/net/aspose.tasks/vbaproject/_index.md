---
title: "Kelas VbaProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.VbaProject. Mewakili VbaProject"
type: docs
weight: 2860
url: /id/net/aspose.tasks/vbaproject/
---
## VbaProject class

Mewakili `VbaProject`.

```csharp
public class VbaProject
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Mendapatkan Argumen Kompilasi bersyarat |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Mendapatkan deskripsi proyek. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Mendapatkan Id Konteks Bantuan proyek |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Mendapatkan nama file bantuan |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Mendapatkan koleksi [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Mendapatkan nama proyek |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Mendapatkan koleksi [`VbaReferenceCollection`](../vbareferencecollection/) |

## Contoh

Menampilkan cara membaca properti proyek VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


