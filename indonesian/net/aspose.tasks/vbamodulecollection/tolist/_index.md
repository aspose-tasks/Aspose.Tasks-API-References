---
title: "VbaModuleCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "VbaModuleCollection metode. Mengonversi objek koleksi menjadi daftar objek VbaModule"
type: docs
weight: 100
url: /id/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Mengonversi objek koleksi menjadi daftar objek [`VbaModule`](../../vbamodule/).

```csharp
public List<VbaModule> ToList()
```

### Nilai Kembali

Daftar objek.

## Contoh

Menampilkan cara mengiterasi modul VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### Lihat Juga

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


