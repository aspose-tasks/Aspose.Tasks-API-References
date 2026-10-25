---
title: "Tsk.BudgetWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Trabajo presupuestado para recursos de trabajo y materiales. Los recursos presupuestados se asignan solo a la tarea de resumen del proyecto"
type: docs
weight: 150
url: /es/net/aspose.tasks/tsk/budgetwork/
---
## Tsk.BudgetWork field

Trabajo presupuestado para recursos de trabajo y materiales. Los recursos presupuestados se asignan solo a la tarea de resumen del proyecto.

```csharp
public static readonly Key<Duration, TaskKey> BudgetWork;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


