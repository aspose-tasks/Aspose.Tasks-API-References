---
title: "HtmlSaveOptions.Pages"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti HtmlSaveOptions. Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat merender tata letak proyek. Semua halaman proyek akan disimpan jika daftar ini kosong"
type: docs
weight: 130
url: /id/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat merender tata letak proyek. Semua halaman proyek akan disimpan jika daftar ini kosong.

```csharp
public List<int> Pages { get; set; }
```

## Contoh

Menampilkan cara mengatur header/judul halaman HTML dengan menggunakan opsi &lt;see cref="P:Aspose.Tasks.Saving.HtmlSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Menentukan apakah nama proyek harus disertakan dalam judul HTML (true secara default)
    IncludeProjectNameInTitle = false,

    // Menentukan apakah nama proyek harus disertakan dalam header halaman HTML (true secara default)
    IncludeProjectNameInPageHeader = false,

    // atur halaman yang akan diekspor
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Lihat Juga

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


