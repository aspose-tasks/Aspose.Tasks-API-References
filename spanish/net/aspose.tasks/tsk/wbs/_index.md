---
title: "Tsk.WBS"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Códigos de estructura de desglose del trabajo WBS"
type: docs
weight: 1130
url: /es/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

Códigos de estructura de desglose del trabajo (WBS).

```csharp
public static readonly Key<string, TaskKey> WBS;
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


