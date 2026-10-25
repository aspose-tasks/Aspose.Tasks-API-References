---
title: "ResourceAssignment.SplitTask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-methode. Splits de taak in twee delen"
type: docs
weight: 770
url: /nl/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Splitst de taak in twee delen.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Het begin van de werkonderbreking waarop gesplitst wordt. |
| einde | DateTime | Het einde van de werkonderbreking waarop gesplitst wordt. |
| kalender | Calendar | De kalender waarop gesplitst wordt. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentOutOfRangeException | Gooit een fout wanneer de startdatum kleiner is dan de toewijzings‑startdatum. |
| ArgumentOutOfRangeException | Gooit een fout wanneer de einddatum groter is dan de toewijzings‑einddatum. |

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


