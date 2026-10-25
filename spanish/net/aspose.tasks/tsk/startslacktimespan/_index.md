---
title: "Tsk.StartSlackTimeSpan"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La duración entre las fechas de Inicio Temprano y Inicio Tardío"
type: docs
weight: 1020
url: /es/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

La duración entre las fechas de Inicio Temprano y Inicio Tardío.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Ejemplos

Muestra cómo leer la propiedad Tsk.StartSlackTimeSpan. La propiedad se calcula, por lo que normalmente no es necesario establecerla explícitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


