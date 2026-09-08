---
title: "Tsk.CostVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La diferencia entre el costo de referencia y el costo total de un recurso o asignación de tarea."
type: docs
weight: 240
url: /es/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

La diferencia entre el costo de referencia y el costo total para una tarea, recurso o asignación.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


