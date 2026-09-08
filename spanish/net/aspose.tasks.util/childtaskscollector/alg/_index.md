---
title: "ChildTasksCollector.Alg"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ChildTasksCollector. Procesa el objeto especificado"
type: docs
weight: 30
url: /es/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Procesa el objeto especificado.

```csharp
public override void Alg(Task el, int level)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | Tarea | Objeto a procesar. |
| nivel | Int32 | Nivel del nodo del árbol. |

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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


