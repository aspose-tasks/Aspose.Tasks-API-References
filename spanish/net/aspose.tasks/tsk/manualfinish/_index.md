---
title: "Tsk.ManualFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Define la finalización programada manualmente de una tarea"
type: docs
weight: 790
url: /es/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Define la finalización programada manualmente de una tarea.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


