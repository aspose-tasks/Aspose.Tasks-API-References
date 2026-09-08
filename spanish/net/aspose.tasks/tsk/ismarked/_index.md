---
title: "Tsk.IsMarked"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Indica si una tarea está marcada para una acción posterior o identificación de algún tipo."
type: docs
weight: 620
url: /es/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Muestra si una tarea está marcada para una acción adicional o identificación de algún tipo.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Observaciones

Aplica solo al formato de archivo mpp.

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


