---
title: "تعداد TimeUnitType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.TimeUnitType. يحدد نوع وحدة الوقت"
type: docs
weight: 2570
url: /ar/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

يحدد نوع وحدة الوقت.

```csharp
public enum TimeUnitType : sbyte
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى أن القيمة غير معرفة يعني أن الحقل لم يتم تعريفه في ملف المشروع الأصلي. |
| Minute | `0` | يشير إلى نوع وحدة الوقت دقيقة. |
| ElapsedMinute | `1` | يشير إلى نوع وحدة الوقت دقيقة المنقضية. |
| Hour | `2` | يشير إلى نوع وحدة الوقت ساعة. |
| ElapsedHour | `3` | يشير إلى نوع وحدة الوقت ساعة المنقضية. |
| Day | `4` | يشير إلى نوع وحدة الوقت يوم. |
| ElapsedDay | `5` | يشير إلى نوع وحدة الوقت يوم المنقضية. |
| Week | `6` | يشير إلى نوع وحدة الوقت أسبوع. |
| ElapsedWeek | `7` | يشير إلى نوع وحدة الوقت أسبوع المنقضية. |
| Month | `8` | يشير إلى نوع وحدة الوقت شهر. |
| ElapsedMonth | `9` | يشير إلى نوع وحدة الوقت شهر المنقضية. |
| Percent | `10` | يشير إلى نوع وحدة الوقت نسبة مئوية. |
| ElapsedPercent | `11` | يشير إلى نوع وحدة الوقت نسبة مئوية المنقضية. |
| Null | `12` | يشير إلى نوع وحدة الوقت فارغ. |
| MinuteEstimated | `13` | يشير إلى نوع وحدة الوقت دقيقة المقدرة. |
| ElapsedMinuteEstimated | `14` | يشير إلى نوع وحدة الوقت دقيقة المقدرة المنقضية. |
| HourEstimated | `15` | يشير إلى نوع وحدة الوقت ساعة المقدرة. |
| ElapsedHourEstimated | `16` | يشير إلى نوع وحدة الوقت ساعة المقدرة المنقضية. |
| DayEstimated | `17` | يشير إلى نوع وحدة الوقت يوم المقدرة. |
| ElapsedDayEstimated | `18` | يشير إلى نوع وحدة الوقت يوم المقدرة المنقضية. |
| WeekEstimated | `19` | يشير إلى نوع وحدة الوقت أسبوع المقدرة. |
| ElapsedWeekEstimated | `20` | يشير إلى نوع وحدة الوقت أسبوع المقدرة المنقضية. |
| MonthEstimated | `21` | يشير إلى نوع وحدة الوقت شهر المقدرة. |
| ElapsedMonthEstimated | `22` | يشير إلى نوع وحدة الوقت شهر المقدرة المنقضية. |
| PercentEstimated | `23` | يشير إلى نوع وحدة الوقت نسبة مئوية المقدرة. |
| ElapsedPercentEstimated | `24` | يشير إلى نوع وحدة الوقت المقدرة بالنسبة المئوية المنقضية. |
| Year | `25` | يشير إلى نوع وحدة الوقت للعام. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يظهر كيفية تحويل مدة زمنية إلى أنواع مختلفة من وحدات الوقت.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// احصل على مهمة لحساب مدتها بصيغ مختلفة
var task = project.RootTask.Children.GetById(1);

// احصل على المدة بالدقائق، الأيام، الساعات، الأسابيع والشهور
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


