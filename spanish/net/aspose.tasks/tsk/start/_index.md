---
title: "Tsk.Start"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha de inicio programada de una tarea."
type: docs
weight: 1010
url: /es/net/aspose.tasks/tsk/start/
---
## Tsk.Start field

La fecha de inicio programada de una tarea.

```csharp
public static readonly Key<DateTime, TaskKey> Start;
```

## Ejemplos

Muestra cómo leer/escribir propiedades de tareas.

```csharp
var project = new Project();

// Agregar tarea y establecer propiedades de la tarea
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


