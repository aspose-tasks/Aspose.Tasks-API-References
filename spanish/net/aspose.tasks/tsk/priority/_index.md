---
title: "Tsk.Priority"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El nivel de importancia asignado a una tarea que a su vez indica cuán fácilmente una tarea o asignación puede retrasarse o dividirse durante la nivelación de recursos."
type: docs
weight: 930
url: /es/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

El nivel de importancia asignado a una tarea, que a su vez indica cuán fácilmente una tarea o asignación puede retrasarse o dividirse durante la nivelación de recursos.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Ejemplos

Muestra cómo leer la prioridad de una tarea.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mostrar prioridades para todas las tareas.
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


