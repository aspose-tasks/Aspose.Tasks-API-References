---
title: "SaveOptions.PageSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur ukuran halaman yang akan dirender Nilai default adalah PageSize.A4"
type: docs
weight: 130
url: /id/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Mendapatkan atau mengatur ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Contoh

Menunjukkan cara mengatur ukuran halaman (bisa menjadi salah satu nilai dari enumerasi &lt;see cref=\"P:Aspose.Tasks.Visualization.TiffCompression\" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Render proyek ke semua ukuran halaman yang telah ditentukan sebelumnya
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### Lihat Juga

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


