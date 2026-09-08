---
title: "Tsk.PercentComplete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El estado actual de una tarea expresado como el porcentaje de la duración de la tarea que se ha completado"
type: docs
weight: 880
url: /es/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

El estado actual de una tarea, expresado como el porcentaje de la duración de la tarea que se ha completado.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Ejemplos

Muestra cómo cambiar el progreso de una tarea actualizando el porcentaje de completado de la tarea.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Acceder a tareas y mostrar el porcentaje de finalización
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


