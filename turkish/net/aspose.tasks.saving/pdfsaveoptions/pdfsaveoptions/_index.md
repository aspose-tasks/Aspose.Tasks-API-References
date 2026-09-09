---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions yapıcı. PDF formatında bir belgeyi kaydetmek için kullanılabilecek PdfSaveOptions sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

[`PdfSaveOptions`](../) sınıfının, bir belgeyi [`PDF`](../../savefileformat/) formatında kaydetmek için kullanılabilecek yeni bir örneğini başlatır.

```csharp
public PdfSaveOptions()
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


