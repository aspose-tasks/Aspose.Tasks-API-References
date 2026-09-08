---
title: "TaskUtils.Apply"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskUtils. Aplica el algoritmo especificado a cada tarea de un árbol"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Aplica el algoritmo especificado a cada tarea de un árbol.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| root | Tarea | Raíz del árbol |
| alg | ITreeAlgorithm`1 | Algoritmo aplicado. |
| nivel | Int32 | Nivel de la tarea raíz. |

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

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


