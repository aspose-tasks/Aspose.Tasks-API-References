---
title: "Tsk.IsPublished"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει αν η τρέχουσα εργασία πρέπει να δημοσιευτεί στον Project Server μαζί με το υπόλοιπο του έργου"
type: docs
weight: 660
url: /el/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Καθορίζει εάν η τρέχουσα εργασία πρέπει να δημοσιευτεί στο Project Server μαζί με το υπόλοιπο του έργου.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


