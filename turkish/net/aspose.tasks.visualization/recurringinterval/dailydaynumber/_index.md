---
title: "RecurringInterval.DailyDayNumber"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RecurringInterval özelliği. Günlük gün numarasını alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/recurringinterval/dailydaynumber/
---
## RecurringInterval.DailyDayNumber property

Günlük gün numarasını alır veya ayarlar.

```csharp
public int DailyDayNumber { get; set; }
```

## Örnekler

İlerleme çizgilerinin günlük yinelenen aralığını nasıl ekleyeceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// günlük desen gün numarasını ayarla
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// günlük ilerleme çizgileri için bir günün çalışma günü olup olmadığını belirten bir değeri ayarla.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Ayrıca Bakınız

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


