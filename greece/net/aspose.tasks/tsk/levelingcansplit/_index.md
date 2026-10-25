---
title: "Tsk.LevelingCanSplit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν η λειτουργία εξισορρόπησης πόρων μπορεί να προκαλέσει διαχωρισμούς στην εναπομείνασα εργασία σε αυτήν την εργασία"
type: docs
weight: 760
url: /el/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Καθορίζει εάν η λειτουργία εξισορρόπησης πόρων μπορεί να προκαλέσει διαχωρισμούς στην υπόλοιπη εργασία αυτής της εργασίας.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


