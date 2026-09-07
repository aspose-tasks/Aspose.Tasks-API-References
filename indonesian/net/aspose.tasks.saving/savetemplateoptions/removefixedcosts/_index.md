---
title: "SaveTemplateOptions.RemoveFixedCosts"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveTemplateOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah semua biaya tetap dari templat proyek harus dihapus"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/savetemplateoptions/removefixedcosts/
---
## SaveTemplateOptions.RemoveFixedCosts property

Mendapatkan atau mengatur nilai yang menunjukkan apakah semua biaya tetap dari templat proyek harus dihapus.

```csharp
public bool RemoveFixedCosts { get; set; }
```

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

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


