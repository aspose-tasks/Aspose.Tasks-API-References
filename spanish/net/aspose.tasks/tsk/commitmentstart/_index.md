---
title: "Tsk.CommitmentStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha de inicio de una entrega. La lectura solo es compatible con formato XML."
type: docs
weight: 180
url: /es/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

La fecha de inicio de una entrega. Lectura compatible solo con formato XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


