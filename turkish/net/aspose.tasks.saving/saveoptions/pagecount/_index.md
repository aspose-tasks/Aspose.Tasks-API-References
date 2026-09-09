---
title: "SaveOptions.PageCount"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Projenin sayfa sayısını alır veya ayarlar."
type: docs
weight: 120
url: /tr/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Projenin sayfa sayısını alır veya ayarlar.

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


