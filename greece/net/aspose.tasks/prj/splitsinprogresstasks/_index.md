---
title: "Prj.SplitsInProgressTasks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν οι εργασίες σε εξέλιξη μπορούν να χωριστούν"
type: docs
weight: 650
url: /el/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

Καθορίζει εάν οι εργασίες σε εξέλιξη μπορούν να χωριστούν.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.SplitsInProgressTasks.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


