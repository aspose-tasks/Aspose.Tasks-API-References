---
title: "RemoveTask.Alg"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод RemoveTask. Ничего не делает"
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/removetask/alg/
---
## RemoveTask.Alg method

Ничего не делать.

```csharp
public void Alg(Task el, int level)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | Задача | Объект для обработки. |
| уровень | Int32 | Уровень узла дерева. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


