---
title: "Интерфейс IMessageHandler"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Интерфейс Aspose.Tasks.IMessageHandler. Представляет обратный вызов результатов уравновешивания ресурсов"
type: docs
weight: 880
url: /ru/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Представляет обратный вызов, получающий результаты уравновешивания ресурсов.

```csharp
public interface IMessageHandler
```

## Методы

| Имя | Описание |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks вызывает этот метод при выводе сообщения. |

## Примеры

Показывает, как уравнивать конкретный ресурс, настраивать параметры уравнивания и просматривать сообщения алгоритма уравнивания.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


