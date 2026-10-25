---
title: "Class LevelingResult"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Leveling.LevelingResult. Rappresenta i risultati del livellamento delle risorse"
type: docs
weight: 960
url: /it/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Rappresenta i risultati del livellamento delle risorse.

```csharp
public sealed class LevelingResult
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LevelingResult](levelingresult/)() | Inizializza una nuova istanza della classe `LevelingResult`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Ottiene un insieme di attività interessate dal livellamento delle risorse. |

## Esempi

Mostra come livellare tutte le risorse del progetto utilizzando le opzioni predefinite.

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

### Vedi anche

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


