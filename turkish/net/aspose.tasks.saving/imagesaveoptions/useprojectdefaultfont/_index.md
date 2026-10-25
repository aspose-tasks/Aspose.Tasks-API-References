---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "İşleme için varsayılan yazı tipinin kullanılmasını belirten bir değeri alır veya ayarlar."
type: docs
weight: 110
url: /tr/net/aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/
---
## ImageSaveOptions.UseProjectDefaultFont property

İşleme için varsayılan yazı tipinin kullanılmasını belirten bir değeri alır veya ayarlar.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Açıklamalar

Değer False olduğunda ve DefaultFontName belirtilmişse, render motoru fallback (yedek) yazı tipi olarak DefaultFontName tarafından belirtilen yazı tipini kullanır. Aksi takdirde, yüklüyse 'Arial' veya 'Generic Sans Serif' yazı tipleri fallback olarak kullanılır. Yedek yazı tipi, bir metin stilinin mevcut işletim sisteminde yüklü olmayan bir yazı tipine başvurduğu proje görünümü oluşturulurken kullanılır. Yazı tipi çözümlemesi üzerinde daha fazla kontrol sağlamak için [`FontResolveCallback`](../fontresolvecallback) geri aramasını kullanabilirsiniz.

### Örnekler

Düzeni ayrı dosyalara kaydetmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.DefaultFontName = "Segoe UI Black";
options.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Proje düzenini ayrı dosyalara kaydet
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Ayrıca Bakınız

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
