---
title: "FontSettings.FontResolveCallback"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FontSettings özelliği. Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri aramayı alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri aramayı alır veya ayarlar.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## Örnekler

Yedek yazı tipini ayarlamak veya belirli bir yazı tipini değiştirmek için kullanıcı tanımlı kod çalıştıran özel yazı tipi çözüm geri aramasının nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // Görünüşe göre tam yazı tipi bulunamadı ve yedek yazı tipi ayarlandı.
        // Yedek yazı tipini geçersiz kılabiliriz.
        args.ResolvedFontName = "Arial";
    }

    // Veya sadece belirli yazı tipini değiştirin:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Ayrıca Bakınız

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


