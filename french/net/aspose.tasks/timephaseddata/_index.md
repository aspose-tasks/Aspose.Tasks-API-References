---
title: "Classe TimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TimephasedData. Représente une donnée à phases temporelles"
type: docs
weight: 2590
url: /fr/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Représente des données à phases temporelles.

```csharp
public class TimephasedData
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Initialise une nouvelle instance de la classe `TimephasedData`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Obtient ou définit la date de fin d'une période de données à phases temporelles. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Obtient ou définit la date de début d'une période de données à phases temporelles. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Obtient ou définit le type d'une donnée à phases temporelles. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Obtient ou définit l'identifiant unique d'une donnée à phases temporelles |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Obtient ou définit l'unité de temps d'une période de données à phases temporelles. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Obtient ou définit la valeur par unité de temps pour une période de données à phases temporelles. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Obtient l'instance Double qui représente la valeur chaîne de cet objet. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Obtient l'instance TimeSpan qui représente la valeur chaîne de cet objet. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Obtient l'instance Double qui représente la valeur chaîne de cet objet pour des données à phases temporelles basées sur l'unité. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Crée et initialise une nouvelle instance de la classe `TimephasedData` pour des données à phases temporelles basées sur le coût. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Crée et initialise une nouvelle instance de la classe `TimephasedData` pour des données à phases temporelles basées sur le coût. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Crée et initialise une nouvelle instance de la classe `TimephasedData` pour des données à phases temporelles basées sur l'unité d'une affectation d'une ressource matérielle. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Crée et initialise une nouvelle instance de la classe `TimephasedData` pour les données temporelles basées sur le travail. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


