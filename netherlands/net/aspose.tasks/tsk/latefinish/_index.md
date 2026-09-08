---
title: "Tsk.LateFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De laatste datum waarop een taak kan eindigen zonder de voltooiing van het project te vertragen"
type: docs
weight: 730
url: /nl/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

De laatste datum waarop een taak kan eindigen zonder de voltooiing van het project te vertragen.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.LateFinish te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


