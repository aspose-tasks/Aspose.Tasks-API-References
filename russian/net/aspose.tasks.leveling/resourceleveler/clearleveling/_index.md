---
title: "ResourceLeveler.ClearLeveling"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceLeveler. Удаляет любые задержки выравнивания, ранее добавленные в проект во время выравнивания ресурсов."
type: docs
weight: 10
url: /ru/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Удаляет любую задержку уравнивания, ранее добавленную к проекту во время уравнивания ресурсов.

```csharp
public static void ClearLeveling(Project project)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект, из которого нужно очистить выравнивание. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Удаляет любую задержку уравнивания, ранее добавленную к указанным задачам во время уравнивания ресурсов.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| задачи | IEnumerable`1 | Перечисление, содержащее задачи, для которых следует очистить задержку выравнивания. |

### См. также

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


