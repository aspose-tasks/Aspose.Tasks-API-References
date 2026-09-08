---
title: "TaskUtils.Apply"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskUtils. Применяет указанный алгоритм к каждой задаче в дереве."
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Применяет указанный алгоритм к каждой задаче дерева.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| root | Задача | Корень дерева |
| alg | ITreeAlgorithm`1 | Применённый алгоритм. |
| уровень | Int32 | Уровень корневой задачи. |

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

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


