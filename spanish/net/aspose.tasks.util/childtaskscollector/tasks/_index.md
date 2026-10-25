---
title: "ChildTasksCollector.Tasks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ChildTasksCollector. Obtiene una lista de tareas de objetos hijo recopiladas"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Obtiene una lista de objetos hijos recopilados (tareas).

```csharp
public List<Task> Tasks { get; }
```

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


