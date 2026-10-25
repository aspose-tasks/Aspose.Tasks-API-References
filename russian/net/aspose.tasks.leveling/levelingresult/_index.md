---
title: "Класс LevelingResult"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Leveling.LevelingResult. Представляет результаты уравновешивания ресурсов"
type: docs
weight: 960
url: /ru/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Представляет результаты уравнивания ресурсов.

```csharp
public sealed class LevelingResult
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LevelingResult](levelingresult/)() | Инициализирует новый экземпляр класса `LevelingResult`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Получает набор задач, затронутых уравновешиванием ресурсов. |

## Примеры

Показывает, как уравнять все ресурсы проекта, используя параметры по умолчанию.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### См. также

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


