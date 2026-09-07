---
title: "Prj.DefaultFinishTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Prj πεδίο. Ο προεπιλεγμένος χρόνος λήξης των νέων εργασιών"
type: docs
weight: 230
url: /el/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

Η προεπιλεγμένη ώρα λήξης των νέων εργασιών.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


