---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-methode. Retourneert de instantie TimephasedDataCollection-klasse die instanties van de TimephasedData-klasse bevat binnen de opgegeven start- en einddatums van het gespecificeerde TimephasedDataType"
type: docs
weight: 720
url: /nl/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Retourneert de instantie [`TimephasedDataCollection`](../../timephaseddatacollection/) klasse die instanties van de [`TimephasedData`](../timephaseddata/) klasse bevat binnen de opgegeven start- en einddatums van het gespecificeerde [`TimePhasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | De startdatum voor de tijdgephaseerde gegevens. |
| einde | DateTime | De einddatum voor de tijdgephaseerde gegevens. |
| timephasedType | TimephasedDataType | Het type tijdgephaseerde gegevens ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Retourwaarde

retourneert een lijst die instanties van de [`TimephasedData`](../../timephaseddata/) klasse bevat.

## Voorbeelden

Toont hoe tijdgephaseerde gegevens van een resource‑toewijzing binnen een datumbereik te genereren.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Stel projecteigenschappen in
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Maak resource‑toewijzing
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Stel Backloaded-contour in, dit verhoogt de taakduur van 6 naar 10 dagen
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// haal tijdgephaseerde gegevens op
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Retourneert een [`TimephasedDataCollection`](../../timephaseddatacollection/) object met de instanties van de [`TimephasedData`](../timephaseddata/) klasse binnen de opgegeven start- en einddatums van AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | De startdatum voor de tijdgephaseerde gegevens. |
| einde | DateTime | De einddatum voor de tijdgephaseerde gegevens. |

### Retourwaarde

retourneert een lijst die instanties van de [`TimephasedData`](../../timephaseddata/) klasse bevat.

## Voorbeelden

Toont hoe tijdgephaseerde gegevens van een resource‑toewijzing binnen een datumbereik te genereren.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Stel projecteigenschappen in
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Maak resource‑toewijzing
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Stel Backloaded-contour in, dit verhoogt de taakduur van 6 naar 10 dagen
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// haal tijdgephaseerde gegevens op
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


