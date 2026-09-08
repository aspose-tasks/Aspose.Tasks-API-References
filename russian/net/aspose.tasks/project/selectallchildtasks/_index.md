---
title: "Project.SelectAllChildTasks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Рекурсивно собирает все дочерние задачи корневой задачи"
type: docs
weight: 1230
url: /ru/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Рекурсивно собирает все дочерние задачи корневой задачи.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Возвращаемое значение

Коллекция задач.

## Примеры

Показывает, как перенумеровать WBS-коды выбранных задач.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// вывод: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// вывод: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### См. также

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


