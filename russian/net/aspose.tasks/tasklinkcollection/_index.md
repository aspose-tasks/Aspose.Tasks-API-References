---
title: "Класс TaskLinkCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskLinkCollection. Представляет коллекцию объектов Task"
type: docs
weight: 2420
url: /ru/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Представляет коллекцию объектов [`Task`](../task/).

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте `TaskLinkCollection`. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Получает родительский проект объекта ResourceAssignmentCollection. Родительский [`Project`](../project/) для этого объекта. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Возвращает экземпляр Finish-Start [`TaskLink`](../tasklink/), который был добавлен в объект TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Возвращает экземпляр [`TaskLink`](../tasklink/), который был добавлен в объект TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Возвращает экземпляр [`TaskLink`](../tasklink/), который был добавлен в объект TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Удаляет связь задачи из проекта. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Преобразует объект TaskLinkCollection в список объектов [`TaskLink`](../tasklink/). |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


