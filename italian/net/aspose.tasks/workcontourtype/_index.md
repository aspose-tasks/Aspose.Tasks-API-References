---
title: "Enum WorkContourType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.WorkContourType. Specifica il contorno di un lavoro"
type: docs
weight: 3610
url: /it/net/aspose.tasks/workcontourtype/
---
## WorkContourType enumeration

Specifica il contorno di un lavoro.

```csharp
public enum WorkContourType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Il valore non era definito nel file di progetto originale. |
| Flat | `0` | Contorno di lavoro piatto. |
| BackLoaded | `1` | Contorno di lavoro caricato sul retro. |
| FrontLoaded | `2` | Contorno di lavoro caricato sul fronte. |
| DoublePeak | `3` | Contorno di lavoro a doppio picco. |
| EarlyPeak | `4` | Contorno di lavoro a picco precoce. |
| LatePeak | `5` | Contorno di lavoro a picco tardivo. |
| Bell | `6` | Contorno di lavoro a campana. |
| Turtle | `7` | Contorno di lavoro a tartaruga. |
| Contoured | `8` | Contorno di lavoro personalizzato. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come impostare diversi contorni di dati temporizzati per le assegnazioni delle risorse.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 1, 3, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 1, 7, 17, 0, 0));

// aggiungi un'attività
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

var resource = project.Resources.Add("Resource");

// aggiungi assegnazione di risorsa
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(8));
resourceAssignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

// Il contorno piatto è il contorno predefinito
Console.WriteLine("Flat contour");

var collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("Turtle contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Turtle);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("BackLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.BackLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("FrontLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.FrontLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("Bell contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Bell);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("EarlyPeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.EarlyPeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("LatePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.LatePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifica contorno
Console.WriteLine("DoublePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.DoublePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


