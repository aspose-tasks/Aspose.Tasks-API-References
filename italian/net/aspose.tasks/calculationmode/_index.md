---
title: "Enum CalculationMode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.CalculationMode enum. Specifica la modalità di calcolo del progetto"
type: docs
weight: 210
url: /it/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

Specifica la modalità di calcolo del progetto.

```csharp
public enum CalculationMode
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuno. Le date e i costi del progetto non vengono ricalcolati in questa modalità. |
| Automatic | `1` | Modalità automatica. Le date e i costi del progetto vengono ricalcolati quando si utilizza questa modalità. |
| Manual | `2` | Modalità manuale. Solo i campi necessari vengono ricalcolati in questa modalità, ad esempio UID e ID degli oggetti. |

## Esempi

Mostra come utilizzare la modalità di calcolo automatico.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// Imposta la data di inizio del progetto e aggiungi nuovi task
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Collega i task
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Verifica che le date siano state ricalcolate
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

Mostra come utilizzare la modalità di calcolo nessuna.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// Aggiungi un nuovo task
var task = project.RootTask.Children.Add("Task");

// Nota che anche gli ID non sono stati calcolati
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// Imposta la proprietà duration
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Mostra come utilizzare la modalità di calcolo manuale.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Imposta la data di inizio del progetto e aggiungi nuovi task
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Le proprietà necessarie sono impostate in modalità manuale
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Quando colleghiamo due task insieme le loro date non vengono ricalcolate in modalità manuale
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// L'inizio del Task 2 non è stato modificato
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


