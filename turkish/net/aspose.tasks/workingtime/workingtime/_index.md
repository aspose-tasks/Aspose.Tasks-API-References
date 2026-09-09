---
title: "WorkingTime.WorkingTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkingTime yapıcı. Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık içeren WorkingTime sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

[`WorkingTime`](../) sınıfının belirtilen başlangıç ve bitiş zamanlarıyla bir aralık içeren yeni bir örneğini başlatır.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fromTime | DateTime | aralık başlangıç zamanı |
| toTime | DateTime | aralık bitiş zamanı |

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

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

[`WorkingTime`](../) sınıfının belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesi içeren yeni bir örneğini başlatır.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fromTime | TimeSpan | TimeSpan yapısı tarafından temsil edilen aralığın başlangıç zamanı. |
| toTime | TimeSpan | TimeSpan yapısı tarafından temsil edilen aralığın bitiş zamanı. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | toTime, toTime argümanına eşit veya daha az olduğunda veya fromTime ile toTime arasındaki aralık 24 saatten büyük olduğunda. |

## Örnekler

WorkingTime ctor'nun aşırı yüklemesi, aralığın başlangıç ve bitişini TimeSpan'ler kullanarak başlatmak için kullanılabilir:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Ayrıca Bakınız

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

[`WorkingTime`](../) sınıfının belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesi içeren yeni bir örneğini başlatır.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fromHours | Int32 | Aralığın başlangıç zamanı, tam sayı saat cinsinden temsil edilir (0-24). |
| toHours | Int32 | Aralığın bitiş zamanı, tam sayı saat cinsinden temsil edilir (0-24). |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | toTime, toTime argümanına eşit veya daha az olduğunda veya fromTime ile toTime arasındaki aralık 24 saatten büyük olduğunda. |

## Örnekler

WorkingTime ctor'nun aşırı yüklemesi, aralığın başlangıç ve bitişini tam saatler kullanarak başlatmak için kullanılabilir:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Çalışma zamanının eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Takvimlerin eşitliği, çalışma zamanının from ve to tarihleriyle karşılaştırılarak kontrol edilir.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Ayrıca Bakınız

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


