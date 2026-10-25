---
title: "Tsk.RemainingOvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El gasto de horas extra programado restante para una tarea."
type: docs
weight: 970
url: /es/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

El gasto restante programado de horas extra para una tarea.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


