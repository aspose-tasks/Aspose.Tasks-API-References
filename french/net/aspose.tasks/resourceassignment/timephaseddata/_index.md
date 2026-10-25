---
title: "ResourceAssignment.TimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ResourceAssignment. Obtient ou définit l'instance de la classe TimephasedDataCollection contenant des éléments de la classe TimephasedData"
type: docs
weight: 600
url: /fr/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Obtient ou définit l'instance de la classe [`TimephasedDataCollection`](../../timephaseddatacollection/) contenant des éléments de la classe `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Exemples

Montre comment lire les données à phases temporelles d'une affectation de ressources.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Créer une affectation de ressource
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// obtenir des données temporelles
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


