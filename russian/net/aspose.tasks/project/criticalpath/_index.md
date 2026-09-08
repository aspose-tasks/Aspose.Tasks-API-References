---
title: "Project.CriticalPath"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает коллекцию, содержащую список критических задач, которые образуют критический путь этого проекта. Это операция On, где n — количество задач в проекте."
type: docs
weight: 180
url: /ru/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Получает коллекцию, содержащую список критических задач, составляющих критический путь этого проекта. Это операция O(n), где n — количество задач в проекте.

```csharp
public TaskCollection CriticalPath { get; }
```

### Возвращаемое значение

коллекция, представляющая список всех критических задач.

## Примеры

Показывает, как вычислить критический путь проекта.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Отобразить критический путь сейчас
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### См. также

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


