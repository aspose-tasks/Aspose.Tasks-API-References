---
title: "Tsk.Type"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tipo de una tarea"
type: docs
weight: 1100
url: /es/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

El tipo de una tarea.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


