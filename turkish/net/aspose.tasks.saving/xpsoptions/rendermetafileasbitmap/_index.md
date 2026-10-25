---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "XpsOptions özelliği. Bir metafilenin bitmap olarak render edilip edilmemesi gerektiğini gösteren bir değeri alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Bir metafilenin bitmap olarak render edilip edilmemesi gerektiğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
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


