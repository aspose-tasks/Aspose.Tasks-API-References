---
title: "Tsk.StartVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo que representa la diferencia entre la fecha de inicio de referencia de una tarea o asignación y su fecha de inicio programada actualmente."
type: docs
weight: 1040
url: /es/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

El tiempo que representa la diferencia entre una fecha de inicio de línea base de una tarea o asignación y su fecha de inicio programada actualmente.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


