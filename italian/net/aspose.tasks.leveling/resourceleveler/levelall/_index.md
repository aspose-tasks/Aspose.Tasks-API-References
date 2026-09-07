---
title: "ResourceLeveler.LevelAll"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceLeveler. Livella le attività per tutte le risorse del progetto utilizzando le opzioni di livellamento predefinite."
type: docs
weight: 20
url: /it/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Livella le attività per tutte le risorse del progetto utilizzando le opzioni di livellamento predefinite.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Progetto a cui applicare il livellamento delle risorse. |

### Valore di ritorno

Oggetto contenente i risultati del livellamento delle risorse.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


