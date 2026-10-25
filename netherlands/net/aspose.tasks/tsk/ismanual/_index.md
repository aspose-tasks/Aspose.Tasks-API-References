---
title: "Tsk.IsManual"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak handmatig gepland is"
type: docs
weight: 610
url: /nl/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Bepaalt of een taak handmatig is gepland.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsManual gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


