---
title: "LevelingOptions.MessageLevel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство LevelingOptions. Получает или задает уровень сообщений журнала, генерируемых Aspose.Tasks во время ресурсного выравнивания"
type: docs
weight: 60
url: /ru/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Получает или задает уровень сообщений журнала, генерируемых Aspose.Tasks во время уравнивания ресурсов.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


