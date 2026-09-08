---
title: "Tsk.LateStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha más reciente en que una tarea puede comenzar sin retrasar la finalización del proyecto"
type: docs
weight: 740
url: /es/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

La fecha más reciente en que una tarea puede iniciar sin retrasar la finalización del proyecto.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


