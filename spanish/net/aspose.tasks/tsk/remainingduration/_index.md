---
title: "Tsk.RemainingDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo necesario para completar la parte no terminada de una tarea."
type: docs
weight: 960
url: /es/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

El tiempo necesario para completar la parte no terminada de una tarea.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


