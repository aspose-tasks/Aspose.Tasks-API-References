---
title: "Tsk.WBSLevel"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El nivel WBS más a la derecha de una tarea"
type: docs
weight: 1140
url: /es/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

El nivel WBS más a la derecha de una tarea.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## Ejemplos

Muestra cómo leer los códigos WBS de la tarea.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


