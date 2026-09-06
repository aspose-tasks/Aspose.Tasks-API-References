---
title: "Duration.ToDouble"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تقوم بتحويل كائن Duration إلى قيمة Double."
type: docs
weight: 110
url: /ar/net/aspose.tasks/duration/todouble/
---
## Duration.ToDouble method

يحوّل كائن Duration إلى قيمة Double.

```csharp
public double ToDouble()
```

### قيمة الإرجاع

القيمة المحوّلة.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


