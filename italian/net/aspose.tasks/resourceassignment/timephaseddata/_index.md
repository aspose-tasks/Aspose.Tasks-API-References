---
title: "ResourceAssignment.TimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ResourceAssignment. Ottiene o imposta l'istanza della classe TimephasedDataCollection contenente gli elementi della classe TimephasedData"
type: docs
weight: 600
url: /it/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Ottiene o imposta l'istanza della classe [`TimephasedDataCollection`](../../timephaseddatacollection/) contenente gli elementi della classe `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Esempi

Mostra come leggere i dati temporizzati di un'assegnazione di risorsa.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Crea un'assegnazione di risorsa
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// ottieni dati timephased
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


