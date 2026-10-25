---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti FontSettings. Mendapatkan atau menetapkan nilai yang menunjukkan apakah font default harus digunakan untuk rendering"
type: docs
weight: 40
url: /id/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Mendapatkan atau mengatur nilai yang menunjukkan apakah font default harus digunakan untuk merender.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Catatan

Ketika nilai adalah False dan DefaultFontName ditentukan, mesin rendering akan menggunakan font yang ditentukan oleh DefaultFontName sebagai font cadangan. Jika tidak, font 'Arial' (jika terpasang) atau font 'Generic Sans Serif' akan digunakan sebagai font cadangan. Font cadangan digunakan selama rendering tampilan proyek ketika gaya teks merujuk pada font yang tidak terpasang di sistem operasi saat ini. Untuk kontrol yang lebih besar atas resolusi font, Anda dapat menggunakan callback [`FontResolveCallback`](../fontresolvecallback/).

## Contoh

Menampilkan cara mengatur font khusus yang akan digunakan untuk mencetak PDF output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Lihat Juga

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


