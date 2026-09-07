---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ResourceLeveler-Methode. Levelt Aufgaben für alle Projektressourcen mit den Standard-Ebenungsoptionen."
type: docs
weight: 20
url: /de/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Levelt Aufgaben für alle Ressourcen des Projekts mit den Standard-Leveling-Optionen.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Projekt | Projekt | Projekt zum Anwenden der Ressourcenebenen. |

### Rückgabewert

Objekt, das die Ergebnisse der Ressourcenebene enthält.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


