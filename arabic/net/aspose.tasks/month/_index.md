---
title: "تعداد Month"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Month. يحدد الشهر."
type: docs
weight: 1040
url: /ar/net/aspose.tasks/month/
---
## Month enumeration

يحدد الشهر.

```csharp
public enum Month
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى أن القيمة لم تُحدد في ملف المشروع الأصلي. |
| January | `0` | يشير إلى شهر يناير. |
| February | `1` | يشير إلى شهر فبراير. |
| March | `2` | يشير إلى شهر مارس. |
| April | `3` | يشير إلى شهر أبريل. |
| May | `4` | يشير إلى شهر مايو. |
| June | `5` | يشير إلى شهر يونيو. |
| July | `6` | يشير إلى شهر يوليو. |
| August | `7` | يشير إلى شهر أغسطس. |
| September | `8` | يشير إلى شهر سبتمبر. |
| October | `9` | يشير إلى شهر أكتوبر. |
| November | `10` | يشير إلى شهر نوفمبر. |
| December | `11` | يشير إلى شهر ديسمبر. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يعرض كيفية العمل مع تكرارات اليوم السنوي أثناء إنشاء مهام متكررة جديدة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


