---
title: "Prj.NewTasksAreManual"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν οι νέες εργασίες δημιουργούνται ως χειροκίνητες"
type: docs
weight: 550
url: /el/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Καθορίζει εάν οι νέες εργασίες δημιουργούνται ως χειροκίνητες.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


