---
title: "Clase TaskUtils"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.TaskUtils. Clase auxiliar que proporciona operaciones útiles con tareas"
type: docs
weight: 2770
url: /es/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Clase auxiliar que proporciona operaciones útiles con tareas.

```csharp
public static class TaskUtils
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Aplica el algoritmo especificado a cada tarea de un árbol. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Construye un nuevo árbol de tareas que cumplen la condición. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Encuentra una tarea que cumple la condición en un árbol de tareas. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Calcula recursivamente el número de tareas hijas de una tarea a través de todos los niveles. |

## Ejemplos

Muestra cómo trabajar con un algoritmo de árbol.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// recopila todas las tareas del proyecto
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// trabaja con tareas como con una lista simple
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Ver también

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


