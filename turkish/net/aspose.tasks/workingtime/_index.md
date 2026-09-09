---
title: "WorkingTime sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WorkingTime sınıfı. Bir hafta içi gününde çalışma süresini temsil eder."
type: docs
weight: 3660
url: /tr/net/aspose.tasks/workingtime/
---
## WorkingTime class

Bir hafta günü içindeki çalışma zamanını temsil eder.

```csharp
public class WorkingTime
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | `WorkingTime` sınıfının yeni bir örneğini belirtilen başlangıç ve bitiş zamanlarıyla bir aralıkla başlatır. |
| [WorkingTime](workingtime/#constructor)(int, int) | `WorkingTime` sınıfının yeni bir örneğini belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesiyle başlatır. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | `WorkingTime` sınıfının yeni bir örneğini belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesiyle başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Bir çalışma süresinin başlangıcını alır. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Bir çalışma süresinin sonunu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Nesnelerin eşit olduğunu kontrol eder. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | `WorkingTime` sınıfının örneği için bir hash kodu değeri döndürür. |

## Örnekler

Çalışma zamanı bilgileriyle nasıl çalışılacağını gösterir.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Bu veri, "Details." düğmesiyle ilgilidir; özel bir Hafta Günü için özel çalışma zamanları ayarlayabilir veya hatta çalışmaz olarak işaretleyebilirsiniz.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Çalışma zamanları arasında daha fazla dolaşabilir ve bunları görüntüleyebilirsiniz.
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


