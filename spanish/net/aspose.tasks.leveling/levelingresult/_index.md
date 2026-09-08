---
title: "Class LevelingResult"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Leveling.LevelingResult class. Representa los resultados del nivelado de recursos"
type: docs
weight: 960
url: /es/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Representa los resultados del nivelado de recursos.

```csharp
public sealed class LevelingResult
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LevelingResult](levelingresult/)() | Inicializa una nueva instancia de la clase `LevelingResult`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Obtiene un conjunto de tareas afectadas por el nivelado de recursos. |

## Ejemplos

Muestra cómo nivelar todos los recursos del proyecto usando opciones predeterminadas.

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

### Ver también

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


