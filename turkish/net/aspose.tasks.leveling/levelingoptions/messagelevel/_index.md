---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LevelingOptions özelliği. Kaynak dengelemesi sırasında Aspose.Tasks tarafından üretilen günlük mesajlarının seviyesini alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Aspose.Tasks tarafından kaynak dengelemesi sırasında yayımlanan günlük mesajlarının seviyesini alır veya ayarlar.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


