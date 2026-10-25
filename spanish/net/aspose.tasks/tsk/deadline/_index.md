---
title: "Tsk.Deadline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Una fecha objetivo que indica cuándo debe completarse una tarea"
type: docs
weight: 270
url: /es/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Una fecha objetivo que indica cuándo debe completarse una tarea.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


