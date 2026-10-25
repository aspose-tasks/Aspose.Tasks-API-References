---
title: "Tsk.ManualStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Define el inicio programado manualmente de una tarea"
type: docs
weight: 800
url: /es/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Define el inicio programado manualmente de una tarea.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


