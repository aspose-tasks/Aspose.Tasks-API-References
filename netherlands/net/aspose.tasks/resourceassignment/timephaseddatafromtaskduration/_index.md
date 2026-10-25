---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment methode. Genereert een lijst met tijdgephaseerde gegevens op basis van de taakduur en de geplande startdatum"
type: docs
weight: 780
url: /nl/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

Genereert een lijst met tijdgephaseerde gegevens op basis van de taakduur en de geplande startdatum.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| kalender | Calendar | De kalender waaruit tijdgephaseerde gegevens worden gegenereerd. |

## Voorbeelden

Toont hoe een splitsing aan een taak kan worden toegevoegd.

```csharp
var project = new Project();

// Haalt een standaardkalender op
var calendar = project.Get(Prj.Calendar);

// Stel de kalendersinstellingen van het project in
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Voeg een nieuwe taak toe aan de hoofdtaak
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Maak een nieuwe resource‑toewijzing aan en genereer tijdgephaseerde gegevens
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Splits de taak in 3 delen.
// Geef startdatum- en einddatumpunten door aan de SplitTask-methode die voor de splitsing worden gebruikt
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


