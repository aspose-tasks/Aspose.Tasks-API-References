---
title: "Enum TaskType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskType enum. Bir görevin türünü belirtir"
type: docs
weight: 2470
url: /tr/net/aspose.tasks/tasktype/
---
## TaskType enumeration

Bir görevin türünü belirtir.

```csharp
public enum TaskType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Tanımsız değer, alanın orijinal dosyada tanımlanmadığı anlamına gelir |
| FixedUnits | `0` | Sabit birimler |
| FixedDuration | `1` | Sabit süre |
| FixedWork | `2` | Sabit iş |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


