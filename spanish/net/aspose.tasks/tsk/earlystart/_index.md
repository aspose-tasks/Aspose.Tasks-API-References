---
title: "Tsk.EarlyStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha más temprana en la que una tarea podría comenzar, basada en las fechas de inicio temprano de las tareas predecesoras y sucesoras y otras restricciones."
type: docs
weight: 340
url: /es/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

La fecha más temprana en que una tarea podría comenzar, basada en las fechas de inicio temprano de tareas predecesoras y sucesoras y otras restricciones.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


