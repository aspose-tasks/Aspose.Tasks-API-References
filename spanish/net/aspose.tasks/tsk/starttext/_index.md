---
title: "Tsk.StartText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Devuelve el texto de inicio de la tarea"
type: docs
weight: 1030
url: /es/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Devuelve el texto de inicio de la tarea.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


