---
title: "Tsk.IsRecurring"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea forma parte de una serie de tareas recurrentes"
type: docs
weight: 670
url: /es/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Determina si una tarea forma parte de una serie de tareas recurrentes.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


