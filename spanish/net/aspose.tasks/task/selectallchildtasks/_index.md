---
title: "Task.SelectAllChildTasks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Task. Recopila recursivamente todas las subtareas de esta tarea"
type: docs
weight: 1400
url: /es/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Recopila recursivamente todas las tareas hijas de esta tarea.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Valor devuelto

Una lista de subtareas de esta tarea.

## Ejemplos

Muestra cómo iterar sobre subtareas.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


