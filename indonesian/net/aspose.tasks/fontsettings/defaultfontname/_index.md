---
title: "FontSettings.DefaultFontName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti FontSettings. Mendapatkan atau menetapkan font default atau cadangan untuk rendering"
type: docs
weight: 20
url: /id/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Mendapatkan atau mengatur font default (atau cadangan) untuk merender.

```csharp
public string DefaultFontName { get; set; }
```

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


