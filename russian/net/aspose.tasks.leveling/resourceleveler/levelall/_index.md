---
title: "ResourceLeveler.LevelAll"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceLeveler. Выравнивает задачи для всех ресурсов проекта, используя параметры выравнивания по умолчанию."
type: docs
weight: 20
url: /ru/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Уравнивает задачи для всех ресурсов проекта, используя параметры уравнивания по умолчанию.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект, к которому применяется выравнивание ресурсов. |

### Возвращаемое значение

Объект, содержащий результаты выравнивания ресурсов.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


