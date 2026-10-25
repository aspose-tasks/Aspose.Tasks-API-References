---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PdfSaveOptions. Menginisialisasi sebuah instance baru dari kelas PdfSaveOptions yang dapat digunakan untuk menyimpan dokumen dalam format PDF"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Menginisialisasi sebuah instance baru dari kelas [`PdfSaveOptions`](../) yang dapat digunakan untuk menyimpan dokumen dalam format [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


