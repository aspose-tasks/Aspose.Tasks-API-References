---
title: "Класс LevelingOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Leveling.LevelingOptions. Позволяет задавать параметры уравнивания ресурсов"
type: docs
weight: 940
url: /ru/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Позволяет указать параметры уравнивания ресурсов.

```csharp
public sealed class LevelingOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Инициализирует новый экземпляр класса `LevelingOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Получает или задает токен, который может использоваться для отмены операции уравнивания проекта. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Получает или задает дату окончания периода уравнивания. Значение по умолчанию — дата завершения проекта. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Получает порядок, в котором алгоритм уравнивания откладывает задачи с переизбытком ресурсов. После определения задач, вызывающих переизбыток, и задач, которые можно отложить, используется указанный порядок, определяющий, какая задача должна быть отложена первой. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Получает или задает обратный вызов обработчика сообщений, который может использоваться для перехвата сообщений журнала, создаваемых Aspose.Tasks во время уравнивания ресурсов. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Получает или задает уровень сообщений журнала, генерируемых Aspose.Tasks во время уравнивания ресурсов. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Получает или задает список ресурсов, которые будут уравнены. Если установить null, будут уравнены все ресурсы проекта. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Получает или задает дату начала периода уравнивания. Значение по умолчанию — дата начала проекта. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


