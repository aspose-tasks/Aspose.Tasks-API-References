---
title: "ResourceAssignment.TimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-eigenschap. Haalt of stelt de instantie van de TimephasedDataCollection-klasse in die elementen van de TimephasedData-klasse bevat"
type: docs
weight: 600
url: /nl/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Haalt of stelt de instantie van de [`TimephasedDataCollection`](../../timephaseddatacollection/) klasse in die elementen van de `TimephasedData` klasse bevat.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Voorbeelden

Toont hoe tijdgephaseerde gegevens van een resource‑toewijzing gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
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
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// haal tijdgephaseerde gegevens op
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


