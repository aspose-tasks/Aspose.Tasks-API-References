---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions özelliği. Proje düzeni oluşturulurken gradient fırçasının kullanılıp kullanılmayacağını gösteren bir değeri alır veya ayarlar. Şu anda HTML'ye render ederken gradient fırçasının kullanımı desteklenmemektedir."
type: docs
weight: 160
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Proje düzeni renderlanırken degrade fırçası kullanılıp kullanılmayacağını gösteren bir değeri alır veya ayarlar. Şu anda HTML'ye renderlanırken degrade fırçası kullanımı desteklenmemektedir.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Örnekler

Projeyi HTML dosyasına dışa aktarırken kullanılacak özel bir yazı tipinin nasıl ayarlanacağını gösterir.

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

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


