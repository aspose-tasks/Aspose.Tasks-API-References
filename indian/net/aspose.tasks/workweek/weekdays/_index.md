---
title: "WorkWeek.WeekDays"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkWeek प्रॉपर्टी। सप्ताह के दिनों को प्राप्त करता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/workweek/weekdays/
---
## WorkWeek.WeekDays property

सप्ताह के दिनों को प्राप्त करता है।

```csharp
public WeekDayCollection WeekDays { get; }
```

## उदाहरण

प्रोजेक्ट से कार्य सप्ताह की जानकारी पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // कार्य सप्ताह का नाम, पैरेंट कैलेंडर का नाम, प्रारंभ और समाप्ति तिथियों को प्रदर्शित करें
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // यह डेटा \"Details.\" बटन के बारे में है; आप विशेष सप्ताह के दिन के लिए विशेष कार्य समय सेट कर सकते हैं या इसे गैर-कार्यात्मक भी बना सकते हैं।
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
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

    Console.WriteLine();
}
```

### संबंधित देखें

* class [WeekDayCollection](../../weekdaycollection/)
* class [WorkWeek](../)
* namespace [Aspose.Tasks](../../workweek/)
* assembly [Aspose.Tasks](../../../)


