---
title: "Класс RemoveTask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.RemoveTask. Удаляет указанную задачу из дерева задач"
type: docs
weight: 2760
url: /ru/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Удаляет указанную задачу из дерева задач.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Инициализирует новый экземпляр класса `RemoveTask`. |

## Методы

| Имя | Описание |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Ничего не делать. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Ничего не делать. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Удаляет задачу из указанной родительской задачи. |

## Примеры

Показывает, как использовать алгоритм на основе дерева &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt;.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // использовать алгоритм на основе дерева для удаления task1 из дерева
    var algorithm = new RemoveTask(task1);

    // применить алгоритм к дереву задач
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // проверить результаты
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### См. также

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


