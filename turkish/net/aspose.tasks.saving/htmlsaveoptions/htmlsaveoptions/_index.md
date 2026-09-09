---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions yapıcı. HtmlSaveOptions sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

[`HtmlSaveOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public HtmlSaveOptions()
```

## Örnekler

Bir projeyi HTML formatında nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// VEYA

// Yalnızca bir sayfa ekleme (sayfa numarası 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


