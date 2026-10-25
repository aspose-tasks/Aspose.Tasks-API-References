---
title: "Prj.DefaultFixedCostAccrual"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο προεπιλεγμένος τύπος όταν τα σταθερά κόστη συσσωρεύονται"
type: docs
weight: 240
url: /el/net/aspose.tasks/prj/defaultfixedcostaccrual/
---
## Prj.DefaultFixedCostAccrual field

Ο προεπιλεγμένος τύπος όταν τα σταθερά κόστη συσσωρεύονται.

```csharp
public static readonly Key<CostAccrualType, PrjKey> DefaultFixedCostAccrual;
```

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


