---
title: "Tsk.ManualStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. Definieert handmatig geplande start van een taak"
type: docs
weight: 800
url: /nl/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Definieert de handmatig geplande start van een taak.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ManualStart te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


