---
title: "Prj.DefaultTaskEVMethod"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Görevler için varsayılan kazanılmış değer yöntemi"
type: docs
weight: 280
url: /tr/net/aspose.tasks/prj/defaulttaskevmethod/
---
## Prj.DefaultTaskEVMethod field

Görevler için varsayılan kazanılmış değer yöntemi.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> DefaultTaskEVMethod;
```

## Örnekler

Projenin varsayılan özelliklerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Varsayılan özellikleri ayarla
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Varsayılan özellikleri göster
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


