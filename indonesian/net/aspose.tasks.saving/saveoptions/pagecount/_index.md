---
title: "SaveOptions.PageCount"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur jumlah halaman proyek."
type: docs
weight: 120
url: /id/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Mendapatkan atau mengatur jumlah halaman proyek.

```csharp
public int PageCount { get; }
```

## Contoh

Menampilkan cara menyimpan halaman terpilih dari sebuah proyek ke file PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// mari periksa jumlah halaman yang dapat diekspor
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


