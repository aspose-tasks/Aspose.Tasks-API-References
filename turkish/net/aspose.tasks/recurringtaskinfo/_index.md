---
title: "Sınıf RecurringTaskInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RecurringTaskInfo sınıfı. Bir projedeki yinelenen görevin ayrıntılarını temsil eder."
type: docs
weight: 1720
url: /tr/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Bir projedeki yineleyen bir görevin ayrıntılarını temsil eder.

```csharp
public class RecurringTaskInfo
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Günlük yineleme deseninin tekrar sayısını alır veya ayarlar. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Günlük yineleme deseni için iş günlerinin kullanılıp kullanılmayacağını gösteren bir değeri alır veya ayarlar. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Yinelenen görevin bir oluşumu için süreyi alır veya ayarlar. [`Duration`](./duration/) sınıfının örneği. |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Oluşumların sona ermesi için tarihi alır veya ayarlar. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Aylık yineleme deseninin gün sayısını alır veya ayarlar. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Ordinal gün kullanıldığında aylık yineleme deseninin gününü alır veya ayarlar. DayOfWeek enumarasyonunun değerlerinden biri olabilir. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Aylık yineleme deseninin ordinal numarasını alır veya ayarlar. [`OrdinalNumber`](../ordinalnumber/) enumarasyonunun değerlerinden biri olabilir. |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Ordinal gün kullanıldığında aylık yineleme deseninin tekrar sayısını alır veya ayarlar. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Aylık yineleme deseninin tekrar sayısını alır veya ayarlar. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Aylık yineleme deseni için ordinal gün kullanılacağını gösteren bir değeri alır veya ayarlar. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Yinelenen görevin oluşum sayısını alır veya ayarlar. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Yinelenen görevin yineleme desenini alır veya ayarlar. [`RecurrencePattern`](./recurrencepattern/) enumarasyonunun değerlerinden biri olabilir. |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Oluşumların başlaması için tarihi alır veya ayarlar. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Bu `RecurringTaskInfo` sınıfının örneğinin üst görevini alır. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Yinelenen görev için bitiş tarihini mi yoksa bir tekrar sayısını mı kullanacağını gösteren bir değeri alır veya ayarlar. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Haftalık yineleme deseninde kullanılan günlerin bir koleksiyonunu alır veya ayarlar. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Haftalık yineleme deseni için tekrar sayısını alır veya ayarlar. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Yıllık yineleme deseni için bir tarihi alır veya ayarlar. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Ordinal gün kullanıldığında yıllık yineleme deseninin bir hafta gününü alır veya ayarlar. DayOfWeek enumarasyonunun değerlerinden biri olabilir. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Ordinal gün kullanıldığında yıllık yineleme deseninin bir ayını alır veya ayarlar. [`Month`](../month/) enumarasyonunun değerlerinden biri olabilir. |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Yıllık yineleme deseninin bir ordinal numarasını alır veya ayarlar. [`OrdinalNumber`](../ordinalnumber/) enumarasyonunun değerlerinden biri olabilir. |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Yıllık yineleme deseni için ordinal gün kullanılacağını gösteren bir değeri alır veya ayarlar. |

## Örnekler

Görevlerin yinelenen bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// görevlerin yinelenen bilgilerini oku
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


