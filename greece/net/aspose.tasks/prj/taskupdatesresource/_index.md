---
title: "Prj.TaskUpdatesResource"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν οι ενημερώσεις των εργασιών ενημερώνουν τους πόρους"
type: docs
weight: 710
url: /el/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

Καθορίζει εάν οι ενημερώσεις στις εργασίες ενημερώνουν τους πόρους.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.TaskUpdatesResource.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


