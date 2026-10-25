---
title: "WorkingTime.WorkingTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ WorkingTime. يهيئ مثالًا جديدًا من فئة WorkingTime بفاصل زمني مع أوقات البدء والانتهاء المحددة"
type: docs
weight: 10
url: /ar/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

يهيئ مثالًا جديدًا من فئة [`WorkingTime`](../) مع فاصل زمني مع أوقات البدء والانتهاء المحددة.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fromTime | DateTime | وقت بدء الفاصل |
| toTime | DateTime | وقت انتهاء الفاصل |

## الأمثلة

يوضح كيفية العمل مع معلومات وقت العمل.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // هذه البيانات تتعلق بالكامل بزر \"Details.\" يمكنك تعيين أوقات عمل خاصة ليوم أسبوع خاص أو حتى جعله غير عامل
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // يمكنك أيضًا التنقل عبر أوقات العمل وعرضها
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### انظر أيضًا

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

يهيئ مثالًا جديدًا من فئة [`WorkingTime`](../) مع عنصر فاصل زمني مع أوقات البدء والانتهاء المحددة.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fromTime | TimeSpan | وقت بدء الفاصل ممثل بواسطة بنية TimeSpan. |
| toTime | TimeSpan | وقت انتهاء الفاصل ممثل بواسطة بنية TimeSpan. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | عندما تكون قيمة toTime أصغر من أو مساوية للمعامل toTime أو عندما يكون الفاصل الزمني بين fromTime و toTime أكبر من 24 ساعة. |

## الأمثلة

يمكن استخدام نسخة الدالة الزائدة للمنشئ WorkingTime لتهيئة بداية ونهاية الفاصل الزمني باستخدام TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### انظر أيضًا

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

يهيئ مثالًا جديدًا من فئة [`WorkingTime`](../) مع عنصر فاصل زمني مع أوقات البدء والانتهاء المحددة.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fromHours | Int32 | وقت بدء الفاصل الزمني ممثل بعدد كامل من الساعات (0-24). |
| toHours | Int32 | وقت انتهاء الفاصل الزمني ممثل بعدد كامل من الساعات (0-24). |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | عندما تكون قيمة toTime أصغر من أو مساوية للمعامل toTime أو عندما يكون الفاصل الزمني بين fromTime و toTime أكبر من 24 ساعة. |

## الأمثلة

يمكن استخدام نسخة الدالة الزائدة للمنشئ WorkingTime لتهيئة بداية ونهاية الفاصل الزمني باستخدام ساعات كاملة:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

يعرض كيفية التحقق من مساواة وقت العمل.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// يتم التحقق من مساواة التقويمات مقابل تواريخ from و to لوقت العمل.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### انظر أيضًا

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


