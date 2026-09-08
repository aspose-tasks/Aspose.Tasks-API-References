---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceLeveler method. Voert leveling uit op taken voor alle resources van het project met de standaard leveling-opties."
type: docs
weight: 20
url: /nl/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Nivelleert taken voor alle resources van een project met standaard nivelleringsopties.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Project om resource-leveling toe te passen. |

### Retourwaarde

Object dat de resultaten van resource-leveling bevat.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


