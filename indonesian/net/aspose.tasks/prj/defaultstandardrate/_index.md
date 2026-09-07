---
title: "Prj.DefaultStandardRate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tarif standar default untuk sumber daya baru"
type: docs
weight: 260
url: /id/net/aspose.tasks/prj/defaultstandardrate/
---
## Prj.DefaultStandardRate field

Tarif standar default untuk sumber daya baru.

```csharp
public static readonly Key<double, PrjKey> DefaultStandardRate;
```

## Contoh

Menampilkan cara membaca properti default proyek.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Atur properti default
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Tampilkan properti default
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


