---
title: "TimephasedData.CreateWorkTimephased"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "TimephasedData metodo. Crea e inizializza una nuova istanza della classe TimephasedData per dati a intervalli di tempo basati sul lavoro"
type: docs
weight: 40
url: /it/net/aspose.tasks/timephaseddata/createworktimephased/
---
## TimephasedData.CreateWorkTimephased method

Crea e inizializza una nuova istanza della classe [`TimephasedData`](../) per dati a intervalli di tempo basati sul lavoro.

```csharp
public static TimephasedData CreateWorkTimephased(int uid, DateTime start, DateTime finish, 
    TimeSpan value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | Int32 | UID dell'attività. |
| inizio | DateTime | data-ora di inizio. |
| fine | DateTime | data-ora di fine. |
| valore | TimeSpan | Valore Timespan. |
| timeUnit | TimeUnitType | Tipo di unità di tempo. |
| tipo | TimephasedDataType | Tipo di dati a intervalli di tempo. |

### Valore di ritorno

Un'istanza della classe [`TimephasedData`](../) per dati a intervalli di tempo basati sul lavoro.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Se è stato specificato un valore di lavoro negativo. |

## Esempi

Mostra come lavorare con dati personalizzati a intervalli temporali.

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// Aggiungiamo tds temporizzati personalizzati.
workAssignment.TimephasedData.Clear();

// aggiungi giorni lavorativi
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// aggiungi fine settimana
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// aggiungi giorni lavorativi
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// aggiungi fine settimana
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### Vedi anche

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)


