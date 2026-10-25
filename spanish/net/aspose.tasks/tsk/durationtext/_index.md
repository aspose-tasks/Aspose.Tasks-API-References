---
title: "Tsk.DurationText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Devuelve el texto de duración de la tarea"
type: docs
weight: 310
url: /es/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Devuelve el texto de duración de la tarea.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


