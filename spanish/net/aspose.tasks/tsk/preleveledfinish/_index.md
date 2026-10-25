---
title: "Tsk.PreleveledFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha de finalización de una tarea tal como estaba antes de que se realizara el nivelado de recursos"
type: docs
weight: 910
url: /es/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

La fecha de finalización de una tarea tal como estaba antes de que se realizara la nivelación de recursos.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


