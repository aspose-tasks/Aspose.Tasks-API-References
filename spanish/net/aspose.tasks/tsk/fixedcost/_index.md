---
title: "Tsk.FixedCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Muestra cualquier gasto de tarea que no sea de recursos"
type: docs
weight: 430
url: /es/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

Muestra cualquier gasto de tarea que no sea de recursos.

```csharp
public static readonly Key<double, TaskKey> FixedCost;
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


