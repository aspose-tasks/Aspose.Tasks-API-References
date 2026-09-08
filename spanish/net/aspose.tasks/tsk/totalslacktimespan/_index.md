---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo que la fecha de finalización de una tarea puede retrasarse sin retrasar la fecha de finalización del proyecto."
type: docs
weight: 1090
url: /es/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

El tiempo que la fecha de finalización de una tarea puede retrasarse sin retrasar la fecha de finalización del proyecto.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Ejemplos

Muestra cómo leer la propiedad Tsk.TotalSlackTimeSpan. La propiedad se calcula, por lo que normalmente no es necesario establecerla explícitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


