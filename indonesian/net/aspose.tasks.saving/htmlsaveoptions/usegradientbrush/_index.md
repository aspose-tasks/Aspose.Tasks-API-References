---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti HtmlSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek. Saat ini penggunaan kuas gradien tidak didukung saat merender ke HTML"
type: docs
weight: 160
url: /id/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek. Saat ini penggunaan kuas gradien tidak didukung saat merender ke HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Contoh

Menampilkan cara mengatur font khusus yang akan digunakan untuk mengekspor proyek ke file HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Lihat Juga

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


