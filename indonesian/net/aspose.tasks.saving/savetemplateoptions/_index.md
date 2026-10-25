---
title: "Kelas SaveTemplateOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.SaveTemplateOptions. Memungkinkan menentukan opsi tambahan saat menyimpan proyek sebagai templat"
type: docs
weight: 2200
url: /id/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Mengizinkan untuk menentukan opsi tambahan saat menyimpan proyek sebagai templat.

```csharp
public class SaveTemplateOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah semua nilai aktual dari templat proyek harus dihapus. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah semua nilai dasar dari templat proyek harus dihapus. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah semua biaya tetap dari templat proyek harus dihapus. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tarif sumber daya dari templat proyek harus dihapus. |

## Contoh

Menampilkan cara menyimpan proyek sebagai templat dengan menggunakan opsi.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// buat opsi penyimpanan templat
// dan sesuaikan propertinya
var options = new SaveTemplateOptions
{
    // atur nilai yang menunjukkan apakah semua biaya tetap dari templat proyek harus dihapus
    RemoveFixedCosts = true,

    // atur nilai yang menunjukkan apakah semua nilai aktual dari templat proyek harus dihapus
    RemoveActualValues = true,

    // atur nilai yang menunjukkan apakah tarif sumber daya dari templat proyek harus dihapus
    RemoveResourceRates = true,

    // atur nilai yang menunjukkan apakah semua nilai dasar dari templat proyek harus dihapus
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Lihat Juga

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


