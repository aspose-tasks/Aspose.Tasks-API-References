---
title: "Class LevelingResult"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Leveling.LevelingResult class. Vertegenwoordigt de resultaten van resource leveling"
type: docs
weight: 960
url: /nl/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Stelt de resultaten van resource-leveling voor.

```csharp
public sealed class LevelingResult
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [LevelingResult](levelingresult/)() | Initialiseert een nieuw exemplaar van de `LevelingResult` class. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Haalt een set taken op die zijn beïnvloed door resource leveling. |

## Voorbeelden

Toont hoe alle resources van een project te nivelleren met standaardopties.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### Zie ook

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


