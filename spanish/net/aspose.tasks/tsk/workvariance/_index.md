---
title: "Tsk.WorkVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La diferencia entre el trabajo base de una tarea y el trabajo actualmente programado."
type: docs
weight: 1160
url: /es/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

La diferencia entre el trabajo de línea base de una tarea y el trabajo programado actualmente.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


