---
title: "Tsk.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Το υπόλοιπο προγραμματισμένο κόστος υπερωριών για μια εργασία."
type: docs
weight: 970
url: /el/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

Το υπόλοιπο προγραμματισμένο κόστος υπερωριών για μια εργασία.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


