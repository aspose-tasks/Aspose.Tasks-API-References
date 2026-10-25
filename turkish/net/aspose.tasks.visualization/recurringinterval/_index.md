---
title: "Sınıf RecurringInterval"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.RecurringInterval sınıfı. Gantt Şeması görünümündeki ilerleme çizgilerinde kullanılan yinelenen aralıkları temsil eder."
type: docs
weight: 3310
url: /tr/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Gantt Çizelgesi görünümündeki ilerleme çizgilerinde kullanılan yinelenen aralıkları temsil eder.

```csharp
public class RecurringInterval
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Günlük gün numarasını alır veya ayarlar. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Günlük ilerleme çizgileri için bir günün çalışma günü olup olmadığını belirten değeri alır veya ayarlar. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Yinelenen aralığı alır veya ayarlar. [`Interval`](./interval/) tipinin herhangi bir değeri olabilir. |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Aylık ilerleme çizgilerini gün bazında gösterip göstermeyeceği değerini alır veya ayarlar. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Aylık ilerleme çizgilerinin gün numarasını alır veya ayarlar. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Aylık ilerleme çizgilerinin ay numarasını alır veya ayarlar. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | İlerleme çizgilerini ilk veya son önceden tanımlı günle gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Aylık ilerleme çizgilerinin ilk veya son gün tipini alır veya ayarlar. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | İlerleme çizgilerinin ay numarasını alır veya ayarlar; bu çizgiler ilk veya son önceden tanımlı günle gösterilir. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Haftalık ilerleme çizgileri için günlerin bir listesini alır. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Haftalık ilerleme çizgileri için hafta numarasını alır veya ayarlar. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


