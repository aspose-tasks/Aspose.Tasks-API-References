---
title: "PdfSaveOptions.Pages"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfSaveOptions. Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. Semua halaman akan disimpan jika daftar ini kosong"
type: docs
weight: 60
url: /id/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. Semua halaman akan disimpan jika daftar ini kosong.

```csharp
public List<int> Pages { get; set; }
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


