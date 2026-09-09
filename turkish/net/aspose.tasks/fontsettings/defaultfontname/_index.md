---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FontSettings özelliği. Render için varsayılan veya yedek yazı tipini alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

İşleme için varsayılan (veya yedek) yazı tipini alır veya ayarlar.

```csharp
public string DefaultFontName { get; set; }
```

## Örnekler

Çıktı PDF'sinin yazdırılması için kullanılacak özel yazı tipinin nasıl ayarlanacağını gösterir.

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

### Ayrıca Bakınız

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


