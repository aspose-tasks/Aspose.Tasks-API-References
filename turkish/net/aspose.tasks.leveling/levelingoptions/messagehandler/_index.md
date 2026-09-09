---
title: "LevelingOptions.MessageHandler"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LevelingOptions özelliği. Kaynak dengelemesi sırasında Aspose.Tasks tarafından üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını alır veya ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Aspose.Tasks tarafından kaynak dengelemesi sırasında üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını alır veya ayarlar.

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


