---
title: "Tsk.Cost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El costo total programado o proyectado para una tarea basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante."
type: docs
weight: 230
url: /es/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

El costo total programado o proyectado para una tarea basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
```

## Ejemplos

Muestra cómo leer los costos de la tarea.

```csharp
var project = new Project();

// Agregar tarea y establecer costo
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Mostrar propiedades relacionadas con el costo de la tarea
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


