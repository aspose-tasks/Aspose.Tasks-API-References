---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions özelliği. CSS stil önekini alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

CSS stil önekini alır veya ayarlar.

```csharp
public string CssStylePrefix { get; set; }
```

## Örnekler

HTML'ye dışa aktarım sırasında kullanılan CSS stilleri için ortak bir önek ayarlamanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


