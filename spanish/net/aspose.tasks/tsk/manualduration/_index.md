---
title: "Tsk.ManualDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Define la duración programada manualmente de una tarea"
type: docs
weight: 780
url: /es/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Define la duración programada manualmente de una tarea.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


