---
title: "Enum TaskType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TaskType enum. Καθορίζει τον τύπο μιας εργασίας"
type: docs
weight: 2470
url: /el/net/aspose.tasks/tasktype/
---
## TaskType enumeration

Καθορίζει τον τύπο μιας εργασίας.

```csharp
public enum TaskType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Η μη ορισμένη τιμή σημαίνει ότι το πεδίο δεν ορίστηκε στο αρχικό αρχείο |
| FixedUnits | `0` | Σταθερές μονάδες |
| FixedDuration | `1` | Σταθερή διάρκεια |
| FixedWork | `2` | Σταθερή εργασία |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις προεπιλεγμένες ιδιότητες του έργου.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Ορίστε προεπιλεγμένες ιδιότητες
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Εμφάνιση προεπιλεγμένων ιδιοτήτων
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


