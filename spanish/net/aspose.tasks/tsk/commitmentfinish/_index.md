---
title: "Tsk.CommitmentFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha de finalización de una entrega.  Lectura compatible solo con formato XML"
type: docs
weight: 170
url: /es/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

La fecha de finalización de una entrega. Lectura compatible solo con formato XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


