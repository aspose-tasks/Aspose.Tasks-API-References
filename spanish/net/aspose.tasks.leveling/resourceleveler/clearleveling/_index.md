---
title: "ResourceLeveler.ClearLeveling"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceLeveler. Elimina cualquier retraso de nivelación que se haya añadido previamente al proyecto durante la nivelación de recursos."
type: docs
weight: 10
url: /es/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Elimina cualquier retraso de nivelado que se haya añadido previamente al proyecto durante el nivelado de recursos.

```csharp
public static void ClearLeveling(Project project)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | Proyecto del que se eliminará la nivelación. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Elimina cualquier retraso de nivelado que se haya añadido previamente a las tareas especificadas durante el nivelado de recursos.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tareas | IEnumerable`1 | El enumerable que contiene las tareas para las que se debe eliminar el retraso de nivelación. |

### Ver también

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


