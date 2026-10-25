---
title: "الفئة WorkingTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WorkingTime. تمثل وقت عمل خلال يوم من أيام الأسبوع"
type: docs
weight: 3660
url: /ar/net/aspose.tasks/workingtime/
---
## WorkingTime class

يمثل وقت عمل خلال يوم من أيام الأسبوع.

```csharp
public class WorkingTime
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | ينشئ مثيلاً جديداً من الفئة `WorkingTime` بفاصل يحتوي على أوقات البدء والانتهاء المحددة. |
| [WorkingTime](workingtime/#constructor)(int, int) | ينشئ مثيلاً جديداً من الفئة `WorkingTime` بعنصر فاصل يحتوي على أوقات البدء والانتهاء المحددة. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | ينشئ مثيلاً جديداً من الفئة `WorkingTime` بعنصر فاصل يحتوي على أوقات البدء والانتهاء المحددة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | يحصل على بداية وقت العمل. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | يحصل على نهاية وقت العمل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | يتحقق من أن الكائنات متساوية. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | يرجع قيمة رمز تجزئة (hash code) للمثيل من الفئة `WorkingTime`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


