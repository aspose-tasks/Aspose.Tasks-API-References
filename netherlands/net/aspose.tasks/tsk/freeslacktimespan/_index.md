---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De tijd waarmee een taak kan worden vertraagd zonder opvolgende taken te vertragen."
type: docs
weight: 450
url: /nl/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

De tijd dat een taak kan worden vertraagd zonder enige opvolgtaken te vertragen.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.FreeSlackTimeSpan te lezen. De eigenschap wordt berekend, dus meestal is het niet nodig deze expliciet in te stellen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


