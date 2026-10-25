---
title: "Tsk.CV"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La diferencia entre el costo de referencia y el costo total de una tarea. Variación de costo  Costo  Costo de referencia"
type: docs
weight: 260
url: /es/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

La diferencia entre el costo de referencia y el costo total para una tarea. Variación de costo = Costo - Costo de referencia

```csharp
public static readonly Key<double, TaskKey> CV;
```

## Ejemplos

Muestra cómo leer los valores de costo de la tarea.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


