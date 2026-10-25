---
title: "Tsk.IsRecurring"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Καθορίζει αν μια εργασία αποτελεί μέρος μιας σειράς επαναλαμβανόμενων εργασιών."
type: docs
weight: 670
url: /el/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Καθορίζει εάν μια εργασία αποτελεί μέρος μιας σειράς επαναλαμβανόμενων εργασιών.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


