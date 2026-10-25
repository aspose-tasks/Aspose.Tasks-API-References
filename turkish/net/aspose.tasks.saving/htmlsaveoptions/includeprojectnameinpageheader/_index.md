---
title: "HtmlSaveOptions.IncludeProjectNameInPageHeader"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions özelliği. Proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
weight: 110
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/
---
## HtmlSaveOptions.IncludeProjectNameInPageHeader property

Proje adının HTML sayfa başlığında yer alıp almayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IncludeProjectNameInPageHeader { get; set; }
```

## Örnekler

HTML sayfa başlığı/başlığını &lt;see cref="P:Aspose.Tasks.Saving.HtmlSaveOptions" /&gt; seçeneklerini kullanarak ayarlamanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Proje adının HTML başlığında dahil edilip edilmeyeceğini belirler (varsayılan olarak true)
    IncludeProjectNameInTitle = false,

    // Proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini belirler  (varsayılan olarak true)
    IncludeProjectNameInPageHeader = false,

    // dışa aktarılacak sayfaları ayarla
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


