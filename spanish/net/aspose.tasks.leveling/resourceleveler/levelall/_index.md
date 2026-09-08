---
title: "ResourceLeveler.LevelAll"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceLeveler. Niveliza tareas para todos los recursos del proyecto usando las opciones de nivelación predeterminadas."
type: docs
weight: 20
url: /es/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Nivela las tareas de todos los recursos del proyecto usando opciones de nivelado predeterminadas.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | Proyecto al que se aplicará la nivelación de recursos. |

### Valor devuelto

Objeto que contiene los resultados de la nivelación de recursos.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


