---
title: "Klasse LevelingResult"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.Leveling.LevelingResult Klasse. Stellt die Ergebnisse der Ressourcen-Leveling dar"
type: docs
weight: 960
url: /de/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Stellt die Ergebnisse des Ressourcen-Levelings dar.

```csharp
public sealed class LevelingResult
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LevelingResult](levelingresult/)() | Initialisiert eine neue Instanz der `LevelingResult` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Ruft eine Menge von Aufgaben ab, die vom Ressourcen-Leveling betroffen sind. |

## Beispiele

Zeigt, wie alle Ressourcen des Projekts mit den Standardoptionen gelevelt werden.

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

### Siehe auch

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


