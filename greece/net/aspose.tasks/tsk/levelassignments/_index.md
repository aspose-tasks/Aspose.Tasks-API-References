---
title: "Tsk.LevelAssignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν η λειτουργία εξισορρόπησης μπορεί να καθυστερήσει και να διαχωρίσει μεμονωμένες εκχωρήσεις προκειμένου να επιλύσει τις υπερβολικές κατανομές"
type: docs
weight: 750
url: /el/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Καθορίζει εάν η λειτουργία εξισορρόπησης μπορεί να καθυστερήσει και να χωρίσει μεμονωμένες αναθέσεις προκειμένου να επιλύσει τις υπερκατανομές.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


