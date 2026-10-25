---
title: "Tsk.BudgetCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Costos presupuestarios para recursos de costo presupuestario. Los recursos presupuestarios se asignan solo a la tarea de resumen del proyecto."
type: docs
weight: 140
url: /es/net/aspose.tasks/tsk/budgetcost/
---
## Tsk.BudgetCost field

Costos presupuestados para recursos de costo presupuestado. Los recursos presupuestados solo se asignan a la tarea de resumen del proyecto.

```csharp
public static readonly Key<decimal, TaskKey> BudgetCost;
```

## Ejemplos

Muestra cómo leer los valores de trabajo/costo presupuestado de tarea/recurso/asignación.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Mostrar trabajo presupuestado y costo presupuestado para la tarea resumen del proyecto
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Mostrar trabajo presupuestado del recurso
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Mostrar costo presupuestado del recurso
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Mostrar trabajo presupuestado y costo presupuestado de la asignación
    foreach (var assignment in tsk.Assignments)
    {
        var resource = assignment.Get(Asn.Resource);
        if (resource == null)
        {
            continue;
        }

        if (resource.Get(Rsc.Type) == ResourceType.Work)
        {
            Console.WriteLine("Assignment BudgetWork = " + assignment.Get(Asn.BudgetWork));
        }
        else
        {
            Console.WriteLine("Assignment BudgetCost = " + assignment.Get(Asn.BudgetCost));
        }
    }
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


