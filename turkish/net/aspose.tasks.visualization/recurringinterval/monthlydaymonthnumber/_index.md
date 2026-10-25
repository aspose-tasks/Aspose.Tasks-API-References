---
title: "RecurringInterval.MonthlyDayMonthNumber"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RecurringInterval özelliği. Aylık ilerleme çizgilerinin ay numarasını alır veya ayarlar"
type: docs
weight: 70
url: /tr/net/aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/
---
## RecurringInterval.MonthlyDayMonthNumber property

Aylık ilerleme çizgilerinin ay numarasını alır veya ayarlar.

```csharp
public int MonthlyDayMonthNumber { get; set; }
```

## Örnekler

İlerleme çizgilerinin yinelenen aralığıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// ilerleme çizgisini okuyalım
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// yinelenen aralığı yeniden tanımlayalım
var newInterval = new RecurringInterval();

// Aylık ilerleme çizgilerini gün bazında gösterip göstermeyeceğini belirten bir değer ayarlayın.
interval.MonthlyDay = true;
// Aylık ilerleme çizgilerinin gün numarasını ayarlayın.
interval.MonthlyDayDayNumber = 1;
// Aylık ilerleme çizgilerinin ay numarasını ayarlayın.
interval.MonthlyDayMonthNumber = 1;
// İlerleme çizgilerini ilk ya da son önceden tanımlı günle gösterip göstermeyeceğini belirten bir değer ayarlayın.
interval.MonthlyFirstLast = true;
// Aylık ilerleme çizgilerinin ilk ya da son gün tipini ayarlayın.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// İlk ya da son önceden tanımlı günle gösterilen ilerleme çizgilerinin ay numarasını ayarlayın.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


