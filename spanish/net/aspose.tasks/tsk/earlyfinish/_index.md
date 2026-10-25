---
title: "Tsk.EarlyFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha más temprana en que una tarea podría terminar, basada en las fechas de finalización temprana de tareas predecesoras y sucesoras, otras restricciones y cualquier retraso de nivelación"
type: docs
weight: 330
url: /es/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

La fecha más temprana en que una tarea podría finalizar, basada en las fechas de finalización temprana de tareas predecesoras y sucesoras, otras restricciones y cualquier retraso de nivelación.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


