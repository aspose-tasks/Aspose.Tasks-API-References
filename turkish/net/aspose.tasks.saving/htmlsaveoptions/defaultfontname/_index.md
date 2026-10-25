---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Renderleme için varsayılan veya yedek yazı tipini alır veya ayarlar."
type: docs
weight: 40
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

İşleme için varsayılan (veya yedek) yazı tipini alır veya ayarlar.

```csharp
public string DefaultFontName { get; set; }
```

### Örnekler

Projeyi HTML dosyasına dışa aktarırken kullanılacak özel bir yazı tipinin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
