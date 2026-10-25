---
title: "Tsk.OutlineNumber"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El número que representa la posición de una tarea en la estructura jerárquica del esquema"
type: docs
weight: 850
url: /es/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

El número que representa la posición de una tarea en la estructura jerárquica del esquema.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
```

## Ejemplos

Muestra cómo leer las propiedades del esquema de la tarea.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


