---
title: "Classe TaskCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TaskCollection. Rappresenta una raccolta di oggetti Task"
type: docs
weight: 2390
url: /it/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Rappresenta una raccolta di oggetti [`Task`](../task/).

```csharp
public class TaskCollection : IList<Task>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Restituisce il numero di oggetti contenuti nella TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Restituisce il progetto genitore dell'oggetto TaskCollection. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Aggiunge un nuovo task alla raccolta dei task del progetto allo stesso livello di outline dell'ultimo task. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Inserisce un nuovo task prima di un task con l'ID specificato e allo stesso livello di outline. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Aggiunge un nuovo task alla raccolta dei task figli. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Aggiungi il task specificato all'istanza della classe `TaskCollection`. Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutti i task del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come slacks, campi di lavoro e costo, ID e livelli di outline). Se ParentProject.CalculationMode è Manual il metodo calcolerà solo l'ID del task, il livello di outline e i numeri di outline automaticamente. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutti i task del progetto (date di inizio/fine, imposta le date anticipate/posticipate, calcola slacks, campi di lavoro e costo, ricalcola ID e livelli di outline). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Aggiunge un nuovo task ricorrente alla raccolta dei task figli. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Verifica se la raccolta contiene l'elemento specificato. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Restituisce un task con l'ID specificato il cui antenato è il task genitore di questa raccolta. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Restituisce un task con l'UID specificato il cui antenato è il task genitore di questa raccolta. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Questa è l'implementazione stub del metodo Insert di IList, che lancia solo NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Questa è l'implementazione stub del metodo Remove di ICollection, che lancia solo NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Converte l'oggetto TaskCollection in un elenco di oggetti [`Task`](../task/). |

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

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


