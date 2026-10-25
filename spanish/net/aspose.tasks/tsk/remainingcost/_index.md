---
title: "Tsk.RemainingCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El gasto programado restante que se incurrirá al completar el trabajo programado restante"
type: docs
weight: 950
url: /es/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

El gasto programado restante que se incurrirá al completar el trabajo programado restante.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
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


