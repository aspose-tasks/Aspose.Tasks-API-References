---
title: "Tsk.FinishVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo que representa la diferencia entre la fecha de finalización de la línea base de una tarea o asignación y su fecha de finalización actual"
type: docs
weight: 420
url: /es/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

El tiempo que representa la diferencia entre la fecha de finalización de referencia de una tarea o asignación y su fecha de finalización actual.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


