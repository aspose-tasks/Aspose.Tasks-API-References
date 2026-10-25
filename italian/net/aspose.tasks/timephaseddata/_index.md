---
title: "Classe TimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TimephasedData. Rappresenta un dato a fasi temporali"
type: docs
weight: 2590
url: /it/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Rappresenta dati a fasi temporali.

```csharp
public class TimephasedData
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Inizializza una nuova istanza della classe `TimephasedData`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Ottiene o imposta la data di fine di un periodo di dati a fasi temporali. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Ottiene o imposta la data di inizio di un periodo di dati a fasi temporali. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Ottiene o imposta il tipo di un dato a fasi temporali. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Ottiene o imposta l'identificatore univoco di un dato a fasi temporali |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Ottiene o imposta l'unità di tempo di un periodo di dati a fasi temporali. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Ottiene o imposta il valore per unità di tempo per un periodo di dati a fasi temporali. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Ottiene l'istanza Double che rappresenta il valore stringa di questo oggetto. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Ottiene l'istanza TimeSpan che rappresenta il valore stringa di questo oggetto. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Ottiene l'istanza Double che rappresenta il valore stringa di questo oggetto per dati a fasi temporali basati su unità. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Crea e inizializza una nuova istanza della classe `TimephasedData` per dati a fasi temporali basati sui costi. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Crea e inizializza una nuova istanza della classe `TimephasedData` per dati a fasi temporali basati sui costi. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Crea e inizializza una nuova istanza della classe `TimephasedData` per dati a fasi temporali basati su unità di un'assegnazione di una risorsa materiale. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Crea e inizializza una nuova istanza della classe `TimephasedData` per dati temporizzati basati sul lavoro. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


