---
title: "Tsk.ManualFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Definieert handmatig geplande einddatum van een taak"
type: docs
weight: 790
url: /nl/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Definieert de handmatig geplande voltooiing van een taak.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ManualFinish gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


