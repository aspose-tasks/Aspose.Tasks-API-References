---
title: "Asn.BudgetWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La cantidad de trabajo presupuestada para recursos de trabajo o materiales en una asignación"
type: docs
weight: 160
url: /es/net/aspose.tasks/asn/budgetwork/
---
## Asn.BudgetWork field

La cantidad de trabajo presupuestada para recursos de trabajo o materiales en una asignación.

```csharp
public static readonly Key<Duration, AsnKey> BudgetWork;
```

## Ejemplos

Muestra cómo leer los valores de trabajo/costo presupuestados de una asignación de recursos.

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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


