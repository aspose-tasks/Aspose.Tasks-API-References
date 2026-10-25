---
title: "Task.Get"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Devuelve el valor al que la propiedad está mapeada en este contenedor"
type: docs
weight: 1340
url: /es/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

Devuelve el valor al que la propiedad está asignada en este contenedor.

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| Parámetro | Descripción |
| --- | --- |
| T | el tipo del valor asignado. |
| key | la clave de propiedad especificada. [`Tsk`](../../tsk/) para obtener la clave de la propiedad. |

### Valor devuelto

el valor al que la propiedad está asignada en este contenedor.

## Ejemplos

Muestra cómo obtener/establecer propiedades de la tarea.

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
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


