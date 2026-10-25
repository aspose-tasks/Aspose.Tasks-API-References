---
title: "Tsk.IsRecurring"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak deel uitmaakt van een reeks terugkerende taken."
type: docs
weight: 670
url: /nl/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Bepaalt of een taak deel uitmaakt van een reeks terugkerende taken.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsRecurring te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


