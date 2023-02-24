---
title: Class WeekDay
second_title: Aspose.Tasks لمرجع .NET API
description: Aspose.Tasks.WeekDay فصل. يمثل يوم من أيام الأسبوع يحدد إما أيام الأسبوع العادية أو أيام الاستثناءات في التقويم.
type: docs
weight: 3180
url: /ar/net/aspose.tasks/weekday/
---
## WeekDay class

يمثل يوم من أيام الأسبوع يحدد إما أيام الأسبوع العادية أو أيام الاستثناءات في التقويم.

```csharp
public class WeekDay
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [WeekDay](weekday/#constructor)() | يقوم بتهيئة مثيل جديد لملف`WeekDay` فئة . |
| [WeekDay](weekday/#constructor_1)(DayType) | يقوم بتهيئة مثيل جديد لملف`WeekDay` فئة بنوع اليوم المحدد. |
| [WeekDay](weekday/#constructor_2)(DayType, IEnumerable&lt;WorkingTime&gt;) | يقوم بتهيئة مثيل جديد لملف`WeekDay` فئة مع نوع اليوم المحدد وقائمة فترات وقت العمل. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | يحصل على نوع اليوم . |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان التاريخ المحدد أو نوع اليوم يعمل. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | الحصول على بداية وقت الاستثناء أو تعيينه. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | الحصول على أو تحديد نهاية وقت الاستثناء . |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | الحصول على مجموعة WorkTimeCollection لمثيل WeekDay هذا . مجموعة أوقات العمل التي تحدد وقت العمل في أيام الأسبوع. |

## طُرق

| اسم | وصف |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | إنشاء يوم عمل افتراضي . |
| [Clone](../../aspose.tasks/weekday/clone/)() | إرجاع نسخة عميقة من يوم الأسبوع. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | إرجاع قيمة تشير إلى ما إذا كان هذا المثيل يساوي كائنًا محددًا. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | إرجاع قيمة رمز تجزئة لمثيل`WeekDay` فئة . |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | إرجاع وقت العمل ليوم أسبوع . |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | يلقي. صافيDayOfWeek ل[`DayType`](./daytype/) . |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | يحدد الفترات الزمنية الافتراضية ليوم الأسبوع المحدد. |

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks](../../aspose.tasks/)
* المجسم [Aspose.Tasks](../../)


