---
title: "Tsk.IsRollup"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν οι πληροφορίες σχετικά με τις γραμμές Gantt των υποεργασιών θα συγκεντρωθούν στη γραμμή σύνοψης της εργασίας."
type: docs
weight: 690
url: /el/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Καθορίζει εάν οι πληροφορίες σχετικά με τις μπαρ Gantt των υποεργασιών θα συγκεντρωθούν στη μπάρα της συνοπτικής εργασίας.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


