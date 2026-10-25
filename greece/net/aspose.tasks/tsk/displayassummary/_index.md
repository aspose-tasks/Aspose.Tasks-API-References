---
title: "Tsk.DisplayAsSummary"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Καθορίζει αν η εργασία πρέπει να εμφανίζεται ως εργασία σύνοψης. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML."
type: docs
weight: 280
url: /el/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Καθορίζει εάν η εργασία πρέπει να εμφανίζεται ως εργασία σύνοψης. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


