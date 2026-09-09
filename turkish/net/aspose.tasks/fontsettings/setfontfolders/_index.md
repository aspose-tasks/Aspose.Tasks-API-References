---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FontSettings yöntemi. Aspose.Tasks'in projeler görünümünü render ederken TrueType yazı tiplerini aradığı klasörleri ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Aspose.Tasks'in projenin görünümünü işlerken TrueType yazı tiplerini aradığı klasörleri ayarlar.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | String[] | TrueType yazı tiplerini içeren klasörlerin bir dizisi. |
| recursive | Boolean | Doğru ise belirtilen klasörler özyinelemeli olarak taranacaktır. |

## Örnekler

Özel yazı tipi klasörünün nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// Açılan projede kullanılan tüm yazı tipleri için TrueType dosyaları MyFonts klasöründe bulunmalıdır.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Ayrıca Bakınız

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


