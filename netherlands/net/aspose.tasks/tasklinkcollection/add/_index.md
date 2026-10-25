---
title: "TaskLinkCollection.Add"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLinkCollection methode. Retourneert een exemplaar van FinishStart TaskLink dat is toegevoegd aan het TaskLinkCollection‑object."
type: docs
weight: 40
url: /nl/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Retourneert een instantie van Finish-Start [`TaskLink`](../../tasklink/) die is toegevoegd aan het TaskLinkCollection object.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pred | Taak | Voorgaande taak. |
| succ | Taak | Opvolgende taak. |

### Retourwaarde

een task link‑instantie die aan dit object is toegevoegd.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentNullException | Als een van de invoertaken gelijk is aan null, wordt ArgumentNullException gegooid. |

## Voorbeelden

Toont hoe te werken met taakkoppelingscollecties.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// haal taken op
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// koppel de taken
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print koppelingen tussen de taken
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// bewerk koppeling via indextoegang
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// verwijder alle taakkoppelingen
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Zie ook

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Retourneert een instantie van [`TaskLink`](../../tasklink/) die is toegevoegd aan het TaskLinkCollection object.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pred | Taak | Voorgaande taak. |
| succ | Taak | Opvolgende taak. |
| linkType | TaskLinkType | Linktype [`TaskLinkType`](../../tasklinktype/) |

### Retourwaarde

een task link‑instantie die aan dit object is toegevoegd.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentNullException | Als een van de invoertaken gelijk is aan null, wordt ArgumentNullException gegooid. |

## Voorbeelden

Toont hoe te werken met taakkoppelingscollecties.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// haal taken op
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// koppel de taken
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print koppelingen tussen de taken
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// bewerk koppeling via indextoegang
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// verwijder alle taakkoppelingen
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Zie ook

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Retourneert een instantie van [`TaskLink`](../../tasklink/) die is toegevoegd aan het TaskLinkCollection object.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pred | Taak | Voorgaande taak. |
| succ | Taak | Opvolgende taak. |
| linkType | TaskLinkType | Linktype [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Linkvertraging [`Duration`](../../duration/). |

### Retourwaarde

een task link die aan dit object is toegevoegd.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentNullException | Als een van de invoertaken gelijk is aan null, wordt ArgumentNullException gegooid. |

## Voorbeelden

Toont hoe te werken met taakkoppelingscollecties.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// haal taken op
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// koppel de taken
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print koppelingen tussen de taken
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// bewerk koppeling via indextoegang
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// verwijder alle taakkoppelingen
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Zie ook

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Dit is de stub-implementatie van de Add-methode van ICollection, die alleen NotSupportedException gooit.

```csharp
public void Add(TaskLink item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | TaskLink | Het item om toe te voegen. |

### Zie ook

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


