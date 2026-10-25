---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions özelliği. Proje adının HTML başlığında yer alıp almayacağını belirten bir değeri alır veya ayarlar."
type: docs
weight: 120
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Proje adının HTML başlığında yer alıp almayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
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


