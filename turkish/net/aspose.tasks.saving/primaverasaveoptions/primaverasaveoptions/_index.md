---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraSaveOptions yapıcı. PrimaveraSaveOptions sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

[`PrimaveraSaveOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public PrimaveraSaveOptions()
```

## Örnekler

Nasıl çalışılacağını gösterir &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Primavera kaydetme seçeneklerini oluştur ve ayarla
var options = new PrimaveraSaveOptions
                  {
                      // Bir aktivitenin ön ekini ve son ekini tanımla
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // Aktivitelerin yeniden numaralandırılmasını kontrol et
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Ayrıca Bakınız

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


