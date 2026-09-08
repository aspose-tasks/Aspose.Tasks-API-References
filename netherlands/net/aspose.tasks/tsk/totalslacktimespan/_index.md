---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De tijd waarmee de einddatum van een taak kan worden vertraagd zonder de einddatum van het project te vertragen."
type: docs
weight: 1090
url: /nl/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

De tijd waarmee de einddatum van een taak kan worden uitgesteld zonder de einddatum van het project te vertragen.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.TotalSlackTimeSpan te lezen. De eigenschap wordt berekend, dus meestal is het niet nodig deze expliciet in te stellen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


