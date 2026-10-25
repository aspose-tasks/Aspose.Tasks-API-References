---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Renderleme için varsayılan veya yedek yazı tipini alır veya ayarlar."
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/defaultfontname/
---
## PdfSaveOptions.DefaultFontName property

İşleme için varsayılan (veya yedek) yazı tipini alır veya ayarlar.

```csharp
public string DefaultFontName { get; set; }
```

### Örnekler

Çıktı PDF'sinin yazdırılması için kullanılacak özel yazı tipinin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true, UseProjectDefaultFont = false, DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
