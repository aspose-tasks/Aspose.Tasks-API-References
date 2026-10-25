---
title: "Clase ChildTasksCollector"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.ChildTasksCollector. Recopila todas las tareas hijas"
type: docs
weight: 2690
url: /es/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Recopila todas las tareas secundarias.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Inicializa una nueva instancia de la clase `ChildTasksCollector`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Obtiene una lista de objetos hijos recopilados (tareas). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Procesa el objeto especificado. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Ejemplos

Muestra cómo iterar sobre todas las tareas en un proyecto como una lista simple.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ver también

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


