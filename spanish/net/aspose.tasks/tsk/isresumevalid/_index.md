---
title: "Tsk.IsResumeValid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea puede reanudarse"
type: docs
weight: 680
url: /es/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Determina si una tarea puede reanudarse.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


