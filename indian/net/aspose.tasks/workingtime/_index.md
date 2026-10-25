---
title: "क्लास WorkingTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WorkingTime क्लास। एक कार्यदिवस के दौरान कार्य समय को दर्शाता है।"
type: docs
weight: 3660
url: /hi/net/aspose.tasks/workingtime/
---
## WorkingTime class

सप्ताह के दिन के दौरान कार्य समय दर्शाता है।

```csharp
public class WorkingTime
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | `WorkingTime` क्लास का एक नया उदाहरण निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल के साथ आरंभ करता है। |
| [WorkingTime](workingtime/#constructor)(int, int) | `WorkingTime` क्लास का एक नया उदाहरण निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल आइटम के साथ आरंभ करता है। |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | `WorkingTime` क्लास का एक नया उदाहरण निर्दिष्ट प्रारंभ और समाप्ति समय के साथ एक अंतराल आइटम के साथ आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | कार्य समय की शुरुआत प्राप्त करता है। |
| [To](../../aspose.tasks/workingtime/to/) { get; } | कार्य समय का अंत प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | जाँचता है कि वस्तुएँ समान हैं। |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | `WorkingTime` क्लास के उदाहरण के लिए हैश कोड मान लौटाता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


