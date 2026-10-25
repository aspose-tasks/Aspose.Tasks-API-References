---
title: "TimephasedData.CreateCostTimephased"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TimephasedData. Crée et initialise une nouvelle instance de la classe TimephasedData pour des données temporelles phasées basées sur le coût"
type: docs
weight: 20
url: /fr/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## CreateCostTimephased(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) {#createcosttimephased_1}

Crée et initialise une nouvelle instance de la classe [`TimephasedData`](../) pour des données temporelles phasées basées sur le coût.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uid | Int32 | UID de la tâche. |
| début | DateTime | date-heure de début. |
| fin | DateTime | date-heure de fin. |
| value | Double | Valeur du coût. |
| timeUnit | TimeUnitType | Type d'unité de temps. |
| type | TimephasedDataType | Type de données temporelles phasées. |

### Valeur de retour

Une instance de la classe [`TimephasedData`](../) pour des données temporelles phasées basées sur le coût.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Si une valeur de coût négative a été spécifiée. |

## Exemples

Montre comment travailler avec des données personnalisées à phases temporelles.

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

// ajoutons des tds personnalisés à phases temporelles
workAssignment.TimephasedData.Clear();

// ajouter des jours ouvrés
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// ajouter le week-end
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

// ajouter des jours ouvrés
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// ajouter le week-end
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

### Voir aussi

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)

---

## CreateCostTimephased(int, DateTime, DateTime, double, TimephasedDataType) {#createcosttimephased}

Crée et initialise une nouvelle instance de la classe [`TimephasedData`](../) pour des données temporelles phasées basées sur le coût.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimephasedDataType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uid | Int32 | UID de la tâche. |
| début | DateTime | date-heure de début. |
| fin | DateTime | date-heure de fin. |
| value | Double | Valeur du coût. |
| type | TimephasedDataType | Type de données temporelles phasées. |

### Valeur de retour

Une instance de la classe [`TimephasedData`](../) pour des données temporelles phasées basées sur le coût.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Si une valeur de coût négative a été spécifiée. |

### Voir aussi

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)


