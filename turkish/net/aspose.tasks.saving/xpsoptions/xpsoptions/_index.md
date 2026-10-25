---
title: "XpsOptions.XpsOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "XpsOptions yapıcı. XpsOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

[`XpsOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public XpsOptions()
```

## Örnekler

Projeyi XPS dosyası olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// XPS kaydetme seçenekleri oluştur ve parametreleri ayarla
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Ayrıca Bakınız

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


