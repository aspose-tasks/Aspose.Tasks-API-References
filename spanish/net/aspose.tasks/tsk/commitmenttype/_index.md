---
title: "Tsk.CommitmentType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea tiene una entrega asociada o una dependencia de una entrega asociada. La lectura solo es compatible con formato XML."
type: docs
weight: 190
url: /es/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Determina si una tarea tiene una entrega asociada o una dependencia de una entrega asociada. Lectura compatible solo con formato XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


