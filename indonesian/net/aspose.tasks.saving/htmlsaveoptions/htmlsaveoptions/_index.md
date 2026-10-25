---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor HtmlSaveOptions. Menginisialisasi instance baru dari kelas HtmlSaveOptions"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Menginisialisasi instance baru dari kelas [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## Contoh

Menampilkan cara menyimpan proyek dalam format HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// ATAU

// Menambahkan hanya satu halaman (nomor halaman 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Lihat Juga

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


