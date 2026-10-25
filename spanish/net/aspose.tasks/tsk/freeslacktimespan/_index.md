---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo que una tarea puede retrasarse sin retrasar ninguna tarea sucesora."
type: docs
weight: 450
url: /es/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

El tiempo que una tarea puede retrasarse sin retrasar ninguna tarea sucesora.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Ejemplos

Muestra cómo leer la propiedad Tsk.FreeSlackTimeSpan. La propiedad se calcula, por lo que normalmente no es necesario establecerla explícitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


