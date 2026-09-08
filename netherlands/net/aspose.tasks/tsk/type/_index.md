---
title: "Tsk.Type"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Het type van een taak"
type: docs
weight: 1100
url: /nl/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Het type van een taak.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Voorbeelden

Toont hoe de Tsk.Type-eigenschap gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


