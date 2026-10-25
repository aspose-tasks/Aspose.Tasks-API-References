---
title: "TaskLinkCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskLinkCollection. Возвращает экземпляр FinishStart TaskLink, который был добавлен в объект TaskLinkCollection."
type: docs
weight: 40
url: /ru/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Возвращает экземпляр Finish-Start [`TaskLink`](../../tasklink/), который был добавлен в объект TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пред | Задача | Задача‑предшественник. |
| след | Задача | Задача‑последователь. |

### Возвращаемое значение

Экземпляр ссылки задачи, который был добавлен в этот объект.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Если любая из входных задач равна null, будет выброшено исключение ArgumentNullException. |

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
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Возвращает экземпляр [`TaskLink`](../../tasklink/), который был добавлен в объект TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пред | Задача | Задача‑предшественник. |
| след | Задача | Задача‑последователь. |
| linkType | TaskLinkType | Тип ссылки [`TaskLinkType`](../../tasklinktype/) |

### Возвращаемое значение

Экземпляр ссылки задачи, который был добавлен в этот объект.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Если любая из входных задач равна null, будет выброшено исключение ArgumentNullException. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Возвращает экземпляр [`TaskLink`](../../tasklink/), который был добавлен в объект TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пред | Задача | Задача‑предшественник. |
| след | Задача | Задача‑последователь. |
| linkType | TaskLinkType | Тип ссылки [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Задержка ссылки [`Duration`](../../duration/). |

### Возвращаемое значение

Ссылка задачи, которая была добавлена в этот объект.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Если любая из входных задач равна null, будет выброшено исключение ArgumentNullException. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | TaskLink | Элемент для добавления. |

### См. также

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


