---
title: "Prj.StartDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία έναρξης ενός έργου"
type: docs
weight: 680
url: /el/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

Η ημερομηνία έναρξης ενός έργου.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


