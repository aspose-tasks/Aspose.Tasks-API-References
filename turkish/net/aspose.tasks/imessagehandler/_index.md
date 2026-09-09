---
title: "Arayüz IMessageHandler"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.IMessageHandler arayüzü. Kaynak dengelemenin sonuçları için bir geri çağrıyı temsil eder."
type: docs
weight: 880
url: /tr/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Kaynak dengelemenin sonuçlarını sağlayan bir geri aramayı temsil eder.

```csharp
public interface IMessageHandler
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks bir mesaj çıktığında bu yöntemi çağırır. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


