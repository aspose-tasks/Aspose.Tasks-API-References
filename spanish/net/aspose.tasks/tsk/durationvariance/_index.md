---
title: "Tsk.DurationVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La diferencia entre la duración de referencia de una tarea y la estimación total de duración actual de una tarea."
type: docs
weight: 320
url: /es/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

La diferencia entre la duración de referencia de una tarea y la duración total (estimación actual) de una tarea.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


