---
title: "SaveOptions.FitContent"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan untuk menyesuaikan kontennya"
type: docs
weight: 50
url: /id/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Mendapatkan atau mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya.

```csharp
public bool FitContent { get; set; }
```

## Contoh

Menampilkan cara mengatur opsi apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Atur opsi fit content menjadi true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


