---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceLeveler yöntemi. Belirtilen kaynaklar için, belirtilen dengeleme seçeneklerini kullanarak görevleri dengeler."
type: docs
weight: 30
url: /tr/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Belirtilen dengeleme seçeneklerini kullanarak belirtilen kaynaklar için görevleri dengeler.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Kaynak dengelemesinin uygulanacağı proje. |
| seçenekler | LevelingOptions | Kaynakların nasıl dengeleneceğini belirten seçenekler. |

### Dönüş Değeri

Kaynak dengelemesinin sonuçlarını içeren nesne.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | eğer options parametresi null ise. |

## Örnekler

Belirli bir kaynağı dengelemeyi, dengeleme seçeneklerini özelleştirmeyi ve dengeleme algoritması mesajlarını incelemeyi gösterir.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### Ayrıca Bakınız

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


