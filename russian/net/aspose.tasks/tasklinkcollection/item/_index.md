---
title: "TaskLinkCollection.Item"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLinkCollection. Возвращает или задает элемент по указанному индексу"
type: docs
weight: 20
url: /ru/net/aspose.tasks/tasklinkcollection/item/
---
## TaskLinkCollection indexer

Возвращает или задает элемент по указанному индексу.

```csharp
public TaskLink this[int index] { get; set; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начинающийся с нуля, для получения или установки. |

### Возвращаемое значение

элемент по указанному индексу.

## Примеры

Показывает, как работать с коллекциями связей задач.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// получить задачи
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// связать задачи
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// вывести ссылки между задачами
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// редактировать связь по индексу
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// удалить все связи задач
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### См. также

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


