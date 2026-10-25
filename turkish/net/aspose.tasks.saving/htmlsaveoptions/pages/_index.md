---
title: "HtmlSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions özelliği. Proje düzeni render edilirken kaydedilecek sayfa numaralarının bir listesini alır veya ayarlar. Bu liste boş ise tüm proje sayfaları kaydedilir."
type: docs
weight: 130
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

Proje düzeni render edilirken kaydedilecek sayfa numaralarının bir listesini alır veya ayarlar. Liste boşsa tüm proje sayfaları kaydedilir.

```csharp
public List<int> Pages { get; set; }
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


