---
title: "Tsk.Deadline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Een streefdatum die aangeeft wanneer een taak voltooid moet zijn"
type: docs
weight: 270
url: /nl/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Een streefdatum die aangeeft wanneer een taak voltooid moet zijn.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.Deadline te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


