---
title: "Tsk.ManualDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Definieert handmatig geplande duur van een taak"
type: docs
weight: 780
url: /nl/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Definieert de handmatig geplande duur van een taak.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ManualDuration gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


