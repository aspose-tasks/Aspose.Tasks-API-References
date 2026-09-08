---
title: "Класс TaskUtils"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.TaskUtils. Вспомогательный класс, предоставляющий полезные операции с задачами"
type: docs
weight: 2770
url: /ru/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Вспомогательный класс, предоставляющий полезные операции с задачами.

```csharp
public static class TaskUtils
```

## Методы

| Имя | Описание |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Применяет указанный алгоритм к каждой задаче дерева. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Создаёт новое дерево задач, удовлетворяющих условию. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Находит задачу, удовлетворяющую условию, в дереве задач. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Рекурсивно вычисляет количество дочерних задач задачи на всех уровнях. |

## Примеры

Показывает, как работать с алгоритмом дерева.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// собрать все задачи проекта
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// работать с задачами как с обычным списком
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### См. также

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


