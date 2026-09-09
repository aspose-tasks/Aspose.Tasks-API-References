---
title: "PrimaveraSaveOptions.ActivityIdPrefix"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraSaveOptions özelliği. Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan öneki alır veya ayarlar."
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/primaverasaveoptions/activityidprefix/
---
## PrimaveraSaveOptions.ActivityIdPrefix property

Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan ön eki alır veya ayarlar.

```csharp
public string ActivityIdPrefix { get; set; }
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


