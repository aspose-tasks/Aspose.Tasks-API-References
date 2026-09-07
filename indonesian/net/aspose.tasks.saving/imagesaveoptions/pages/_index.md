---
title: "ImageSaveOptions.Pages"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. Semua halaman akan disimpan jika daftar ini kosong"
type: docs
weight: 50
url: /id/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. Semua halaman akan disimpan jika daftar ini kosong.

```csharp
public List<int> Pages { get; set; }
```

## Contoh

Menampilkan cara menyimpan halaman yang dipilih sebagai gambar.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### Lihat Juga

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


