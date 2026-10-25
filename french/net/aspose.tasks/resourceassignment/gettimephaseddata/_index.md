---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Retourne l'instance de la classe TimephasedDataCollection contenant des instances de la classe TimephasedData dans les dates de début et de fin données du TimephasedDataType spécifié"
type: docs
weight: 720
url: /fr/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Retourne l'instance [`TimephasedDataCollection`](../../timephaseddatacollection/) de la classe contenant des instances de la classe [`TimephasedData`](../timephaseddata/) dans les dates de début et de fin données du [`TimephasedDataType`](../../timephaseddatatype/) spécifié.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date de début pour les données à phase temporelle. |
| fin | DateTime | La date de fin pour les données à phase temporelle. |
| timephasedType | TimephasedDataType | Le type de données à phase temporelle ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Valeur de retour

renvoie une liste qui contient des instances de la classe [`TimephasedData`](../../timephaseddata/).

## Exemples

Montre comment générer des données temporelles d'une affectation de ressource dans une plage de dates.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Définir les propriétés du projet
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

// Définir le contour Backloaded, il augmente la durée de la tâche de 6 à 10 jours
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// obtenir des données temporelles
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Retourne l'objet [`TimephasedDataCollection`](../../timephaseddatacollection/) avec les instances de la classe [`TimephasedData`](../timephaseddata/) dans les dates de début et de fin données de AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date de début pour les données à phase temporelle. |
| fin | DateTime | La date de fin pour les données à phase temporelle. |

### Valeur de retour

renvoie une liste contenant des instances de la classe [`TimephasedData`](../../timephaseddata/).

## Exemples

Montre comment générer des données temporelles d'une affectation de ressource dans une plage de dates.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Définir les propriétés du projet
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

// Définir le contour Backloaded, il augmente la durée de la tâche de 6 à 10 jours
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// obtenir des données temporelles
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


