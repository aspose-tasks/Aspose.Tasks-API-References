---
title: "Prj.NewTaskStartDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο προεπιλεγμένος τύπος ημερομηνίας έναρξης για νέες εργασίες"
type: docs
weight: 580
url: /el/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Ο προεπιλεγμένος τύπος ημερομηνίας έναρξης για νέες εργασίες.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Παραδείγματα

Δείχνει πώς να ορίσετε ιδιότητες για νέες εργασίες.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


