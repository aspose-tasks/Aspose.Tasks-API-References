---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Çalışma dışı zaman rengini alır veya ayarlar."
type: docs
weight: 110
url: /tr/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Çalışma dışı zaman rengini alır veya ayarlar.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Örnekler

Çalışma dışı zaman için özel renk ayarlamanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


