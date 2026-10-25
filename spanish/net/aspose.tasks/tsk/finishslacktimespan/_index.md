---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La duración entre las fechas de Finalización Temprana y Finalización Tardía"
type: docs
weight: 400
url: /es/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

La duración entre las fechas de Finalización Temprana y Finalización Tardía.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Ejemplos

Muestra cómo leer la propiedad Tsk.FinishSlackTimeSpan. La propiedad se calcula, por lo que normalmente no es necesario establecerla explícitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


