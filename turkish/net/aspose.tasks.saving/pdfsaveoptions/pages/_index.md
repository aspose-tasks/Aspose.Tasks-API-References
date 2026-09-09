---
title: "PdfSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions özelliği. Proje düzenini ayrı dosyalara kaydederken kaydedilecek sayfa numaralarının listesini alır veya ayarlar. Liste boş ise tüm sayfalar kaydedilir"
type: docs
weight: 60
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini alır veya ayarlar. Liste boşsa tüm sayfalar kaydedilir.

```csharp
public List<int> Pages { get; set; }
```

## Örnekler

Bir projenin seçilen sayfalarını PDF dosyasına nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// dışa aktarılabilecek sayfa sayısını kontrol edelim
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


