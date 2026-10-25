---
title: "Tsk.PreleveledStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha de inicio de una tarea tal como estaba antes de que se realizara el nivelado de recursos"
type: docs
weight: 920
url: /es/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

La fecha de inicio de una tarea tal como estaba antes de que se realizara la nivelación de recursos.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


