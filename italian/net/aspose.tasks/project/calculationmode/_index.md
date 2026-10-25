---
title: "Project.CalculationMode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene o imposta la modalità di calcolo di un progetto. Può essere uno dei valori dell'enumerazione CalculationMode"
type: docs
weight: 110
url: /it/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Ottiene o imposta la modalità di calcolo di un progetto. Può essere uno dei valori dell'enumerazione `CalculationMode`.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Esempi

Mostra come utilizzare la modalità di calcolo del progetto.

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

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


