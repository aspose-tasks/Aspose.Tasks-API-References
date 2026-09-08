---
title: "Класс ChildTasksCollector"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.ChildTasksCollector. Сбирает все дочерние задачи"
type: docs
weight: 2690
url: /ru/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Собирает все дочерние задачи.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Инициализирует новый экземпляр класса `ChildTasksCollector`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Получает список собранных дочерних объектов (задач). |

## Методы

| Имя | Описание |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Обрабатывает указанный объект. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Примеры

Показывает, как перебрать все задачи в проекте в виде простого списка.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### См. также

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


