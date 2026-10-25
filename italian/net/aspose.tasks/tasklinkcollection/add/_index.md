---
title: "TaskLinkCollection.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskLinkCollection. Restituisce un'istanza di FinishStart TaskLink che è stata aggiunta all'oggetto TaskLinkCollection"
type: docs
weight: 40
url: /it/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Restituisce un'istanza di Finish-Start [`TaskLink`](../../tasklink/) che è stata aggiunta all'oggetto TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pred | Attività | Attività predecessore. |
| succ | Attività | Attività successore. |

### Valore di ritorno

un'istanza di collegamento attività che è stata aggiunta a questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Se uno qualsiasi dei task di input è uguale a null, verrà generata un'ArgumentNullException. |

## Esempi

Mostra come lavorare con collezioni di collegamenti di attività.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// ottieni attività
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// collega le attività
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// stampa i collegamenti tra le attività
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifica il collegamento tramite accesso per indice
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// rimuovi tutti i collegamenti di attività
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Vedi anche

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Restituisce un'istanza di [`TaskLink`](../../tasklink/) che è stata aggiunta all'oggetto TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pred | Attività | Attività predecessore. |
| succ | Attività | Attività successore. |
| linkType | TaskLinkType | Tipo di collegamento [`TaskLinkType`](../../tasklinktype/) |

### Valore di ritorno

un'istanza di collegamento attività che è stata aggiunta a questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Se uno qualsiasi dei task di input è uguale a null, verrà generata un'ArgumentNullException. |

## Esempi

Mostra come lavorare con collezioni di collegamenti di attività.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// ottieni attività
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// collega le attività
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// stampa i collegamenti tra le attività
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifica il collegamento tramite accesso per indice
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// rimuovi tutti i collegamenti di attività
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Vedi anche

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Restituisce un'istanza di [`TaskLink`](../../tasklink/) che è stata aggiunta all'oggetto TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pred | Attività | Attività predecessore. |
| succ | Attività | Attività successore. |
| linkType | TaskLinkType | Tipo di collegamento [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Ritardo del collegamento [`Duration`](../../duration/). |

### Valore di ritorno

un collegamento attività che è stato aggiunto a questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Se uno qualsiasi dei task di input è uguale a null, verrà generata un'ArgumentNullException. |

## Esempi

Mostra come lavorare con collezioni di collegamenti di attività.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// ottieni attività
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// collega le attività
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// stampa i collegamenti tra le attività
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifica il collegamento tramite accesso per indice
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// rimuovi tutti i collegamenti di attività
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Vedi anche

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | TaskLink | L'elemento da aggiungere. |

### Vedi anche

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


