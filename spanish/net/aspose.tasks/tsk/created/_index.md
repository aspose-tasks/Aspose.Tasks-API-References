---
title: "Tsk.Created"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha en que se creó una tarea"
type: docs
weight: 250
url: /es/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

La fecha en que se creó una tarea.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


