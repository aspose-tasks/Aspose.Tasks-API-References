---
title: "Tsk.FinishText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Devuelve el texto de finalización de la tarea"
type: docs
weight: 410
url: /es/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Devuelve el texto de finalización de la tarea.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


