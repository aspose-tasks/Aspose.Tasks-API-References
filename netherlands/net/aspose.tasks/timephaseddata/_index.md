---
title: "Klasse TimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TimephasedData klasse. Vertegenwoordigt een tijdsfasegegevens"
type: docs
weight: 2590
url: /nl/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Stelt een tijdgephaseerde gegevens voor.

```csharp
public class TimephasedData
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Initialiseert een nieuw exemplaar van de `TimephasedData` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Haalt op of stelt de einddatum in van een tijdsfasegegevensperiode. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Haalt op of stelt de startdatum in van een tijdsfasegegevensperiode. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Haalt op of stelt het type in van een tijdsfasegegevens. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Haalt op of stelt de unieke identifier in van een tijdsfasegegevens |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Haalt op of stelt de tijdseenheid in van een tijdsfasegegevensperiode. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Haalt op of stelt de waarde per tijdseenheid in voor een tijdsfasegegevensperiode. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Haalt een Double-instantie op die de tekenreekswaarde van dit object vertegenwoordigt. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Haalt een TimeSpan-instantie op die de tekenreekswaarde van dit object vertegenwoordigt. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Haalt een Double-instantie op die de tekenreekswaarde van dit object vertegenwoordigt voor een eenheidsgebaseerde tijdsfasegegevens. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Maakt een nieuw exemplaar van de `TimephasedData` klasse aan en initialiseert deze voor kostengebaseerde tijdsfasegegevens. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Maakt een nieuw exemplaar van de `TimephasedData` klasse aan en initialiseert deze voor kostengebaseerde tijdsfasegegevens. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Maakt een nieuw exemplaar van de `TimephasedData` klasse aan en initialiseert deze voor eenheidsgebaseerde tijdsfasegegevens van een toewijzing van een materiële resource. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Maakt en initialiseert een nieuw exemplaar van de `TimephasedData`-klasse voor werkgebaseerde tijdgephaseerde gegevens. |

## Voorbeelden

Toont hoe te werken met aangepaste tijdgephaseerde gegevens.

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

// laten we aangepaste tijdgephaseerde tds toevoegen
workAssignment.TimephasedData.Clear();

// werkdagen toevoegen
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// weekend toevoegen
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

// werkdagen toevoegen
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// weekend toevoegen
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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


