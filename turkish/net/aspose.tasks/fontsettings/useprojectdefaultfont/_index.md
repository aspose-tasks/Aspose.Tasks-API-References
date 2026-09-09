---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FontSettings özelliği. Varsayılan yazı tipinin render için kullanılıp kullanılmayacağını belirten bir değeri alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

İşleme için varsayılan yazı tipinin kullanılmasını belirten bir değeri alır veya ayarlar.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Açıklamalar

Değer False olduğunda ve DefaultFontName belirtildiğinde, render motoru yedek font olarak DefaultFontName tarafından belirtilen fontu kullanır. Aksi takdirde 'Arial' (kuruluysa) veya 'Generic Sans Serif' fontları yedek font olarak kullanılır. Yedek font, bir metin stili mevcut işletim sisteminde yüklü olmayan bir fonta referans verdiğinde proje görünümünün render edilmesi sırasında kullanılır. Font çözümlemesi üzerinde daha fazla kontrol için [`FontResolveCallback`](../fontresolvecallback/) geri çağrısını kullanabilirsiniz.

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


