---
title: "TaskCollection.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskCollection. Aggiunge il task specificato all'istanza della classe TaskCollection. Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate dopo aver usato questo metodo. Verrà riprogrammata la data di inizio/fine di tutti i task del progetto, impostate le date anticipate/posticipate e calcolati i campi dipendenti come slacks, lavoro e costi, ID e livelli di outline. Se ParentProject.CalculationMode è Manual il metodo calcolerà solo l'ID del task, il livello di outline e i numeri di outline automaticamente. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutti i task del progetto, date di inizio/fine, imposta le date anticipate/posticipate, calcola slacks, lavoro e costi, ricalcola ID e livelli di outline."
type: docs
weight: 50
url: /it/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Aggiunge il task specificato all'istanza della classe [`TaskCollection`](../). Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Verrà riprogrammata tutti i task del progetto (date di inizio/fine, impostazione delle date anticipate/posticipate) e calcolati i campi dipendenti come slacks, lavoro e costi, ID e livelli di outline). Se ParentProject.CalculationMode è Manual il metodo calcolerà solo l'ID del task, il livello di outline e i numeri di outline automaticamente. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutti i task del progetto (date di inizio/fine, impostazione delle date anticipate/posticipate, calcola slacks, lavoro e costi, ricalcola ID e livelli di outline).

```csharp
public void Add(Task item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | Attività | l'attività specificata che dovrebbe essere aggiunta a questa raccolta di attività. |

## Esempi

Mostra come spostare un'attività sotto un altro genitore.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Ottieni attività per ID
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Aggiunta dell'attività 6 a un altro genitore
task2.Children.Add(task);
```

### Vedi anche

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Aggiunge un nuovo task alla raccolta dei task del progetto allo stesso livello di outline dell'ultimo task.

```csharp
public Task Add()
```

### Valore di ritorno

restituisce la nuova istanza aggiunta della classe [`Task`](../../task/).

## Esempi

Mostra come lavorare con le raccolte di task.

```csharp
var project = new Project();

// la raccolta di task non è di sola lettura e può essere estesa
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// crea task
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// stampa i task del progetto
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// un task può essere prelevato dalla raccolta per ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// o per UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// è anche possibile aggiungere un task ricorrente
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// viene restituito il primo task in una sequenza
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// la raccolta può essere convertita in un elenco semplice
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Vedi anche

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Aggiunge un nuovo task alla raccolta dei task figli.

```csharp
public Task Add(string taskName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskName | Stringa | il nome dell'attività specificata. |

### Valore di ritorno

restituisce la nuova istanza aggiunta della classe [`Task`](../../task/).

## Esempi

Mostra come lavorare con le raccolte di task.

```csharp
var project = new Project();

// la raccolta di task non è di sola lettura e può essere estesa
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// crea task
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// stampa i task del progetto
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// un task può essere prelevato dalla raccolta per ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// o per UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// è anche possibile aggiungere un task ricorrente
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// viene restituito il primo task in una sequenza
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// la raccolta può essere convertita in un elenco semplice
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Vedi anche

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Aggiunge un nuovo task ricorrente alla raccolta dei task figli.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskName | Stringa | il nome dell'attività specificata. |
| beforeTaskId | Int32 | L'ID specificato di un'attività prima della quale verrà inserita una nuova attività. |

### Valore di ritorno

restituisce un'attività che è stata inserita prima di un'attività con l'ID specificato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException viene sollevata se l'ID specificato non è un ID di attività valido. |

## Esempi

Mostra come lavorare con le raccolte di task.

```csharp
var project = new Project();

// la raccolta di task non è di sola lettura e può essere estesa
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// crea task
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// stampa i task del progetto
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// un task può essere prelevato dalla raccolta per ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// o per UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// è anche possibile aggiungere un task ricorrente
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// viene restituito il primo task in una sequenza
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// la raccolta può essere convertita in un elenco semplice
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Vedi anche

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Inserisce un nuovo task prima di un task con l'ID specificato e allo stesso livello di outline.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| parameters | RecurringTaskParameters | I parametri specificati per la creazione di un'attività ricorrente. |

### Valore di ritorno

restituisce la nuova istanza aggiunta della classe [`Task`](../../task/).

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Viene lanciata se i parametri specificati sono null. |
| ArgumentException | Viene lanciata se i parametri specificati non sono validi. |

## Esempi

Mostra come lavorare con le raccolte di task.

```csharp
var project = new Project();

// la raccolta di task non è di sola lettura e può essere estesa
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// crea task
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// stampa i task del progetto
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// un task può essere prelevato dalla raccolta per ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// o per UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// è anche possibile aggiungere un task ricorrente
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// viene restituito il primo task in una sequenza
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// la raccolta può essere convertita in un elenco semplice
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Vedi anche

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


