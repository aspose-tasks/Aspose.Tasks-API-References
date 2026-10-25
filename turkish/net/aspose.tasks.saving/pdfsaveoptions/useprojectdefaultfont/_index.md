---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "İşleme için varsayılan yazı tipinin kullanılmasını belirten bir değeri alır veya ayarlar."
type: docs
weight: 120
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/
---
## PdfSaveOptions.UseProjectDefaultFont property

İşleme için varsayılan yazı tipinin kullanılmasını belirten bir değeri alır veya ayarlar.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Açıklamalar

Değer False olduğunda ve DefaultFontName belirtilmişse, render motoru fallback (yedek) yazı tipi olarak DefaultFontName tarafından belirtilen yazı tipini kullanır. Aksi takdirde, yüklüyse 'Arial' veya 'Generic Sans Serif' yazı tipleri fallback olarak kullanılır. Yedek yazı tipi, bir metin stilinin mevcut işletim sisteminde yüklü olmayan bir yazı tipine başvurduğu proje görünümü oluşturulurken kullanılır. Yazı tipi çözümlemesi üzerinde daha fazla kontrol sağlamak için [`FontResolveCallback`](../fontresolvecallback) geri aramasını kullanabilirsiniz.

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
