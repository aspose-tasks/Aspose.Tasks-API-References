---
title: "WorkingTime.WorkingTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkingTime कन्स्ट्रक्टर। निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल के साथ WorkingTime क्लास का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

[`WorkingTime`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल होता है।

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fromTime | DateTime | अंतराल प्रारंभ समय |
| toTime | DateTime | अंतराल समाप्ति समय |

## उदाहरण

कार्य समय जानकारी के साथ काम करने का तरीका दर्शाता है।

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // यह डेटा \"Details.\" बटन के बारे में है; आप विशेष सप्ताह के दिन के लिए विशेष कार्य समय सेट कर सकते हैं या इसे गैर-कार्यात्मक भी बना सकते हैं।
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // आप कार्य समयों के माध्यम से आगे नेविगेट कर सकते हैं और इन्हें प्रदर्शित कर सकते हैं।
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

### संबंधित देखें

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

[`WorkingTime`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल आइटम होता है।

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fromTime | TimeSpan | अंतराल का प्रारंभ समय TimeSpan स्ट्रक्ट द्वारा दर्शाया गया है। |
| toTime | TimeSpan | अंतराल का समाप्ति समय TimeSpan स्ट्रक्ट द्वारा दर्शाया गया है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | जब toTime, toTime तर्क से कम या बराबर हो, या जब fromTime और toTime के बीच अंतराल 24 घंटे से अधिक हो। |

## उदाहरण

WorkingTime ctor का ओवरलोड अंतराल की शुरुआत और अंत को TimeSpans का उपयोग करके प्रारंभ करने के लिए उपयोग किया जा सकता है:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### संबंधित देखें

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

[`WorkingTime`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल आइटम होता है।

```csharp
public WorkingTime(int fromHours, int toHours)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fromHours | Int32 | अंतराल का प्रारंभ समय पूर्ण घंटों (0-24) में दर्शाया गया है। |
| toHours | Int32 | अंतराल का समाप्ति समय पूर्ण घंटों (0-24) में दर्शाया गया है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | जब toTime, toTime तर्क से कम या बराबर हो, या जब fromTime और toTime के बीच अंतराल 24 घंटे से अधिक हो। |

## उदाहरण

WorkingTime ctor का ओवरलोड अंतराल की शुरुआत और अंत को पूर्ण घंटों का उपयोग करके प्रारंभ करने के लिए उपयोग किया जा सकता है:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

दिखाता है कि कार्य समय समानता की जाँच कैसे करें।

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// कैलेंडरों की समानता को कार्य समय की from और to तिथियों के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### संबंधित देखें

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


