---
title: "WorkWeekCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkWeekCollection मेथड। WorkWeekCollection ऑब्जेक्ट को WorkWeek वस्तुओं की सूची में परिवर्तित करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/workweekcollection/tolist/
---
## WorkWeekCollection.ToList method

WorkWeekCollection ऑब्जेक्ट को [`WorkWeek`](../../workweek/) वस्तुओं की सूची में परिवर्तित करता है।

```csharp
public List<WorkWeek> ToList()
```

### रिटर्न वैल्यू

[`WorkWeek`](../../workweek/) वस्तुओं की सूची।

## उदाहरण

कैलेंडर के लिए एक कस्टम कार्य सप्ताह बनाने का तरीका दिखाता है।

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

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
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

* class [WorkWeek](../../workweek/)
* class [WorkWeekCollection](../)
* namespace [Aspose.Tasks](../../workweekcollection/)
* assembly [Aspose.Tasks](../../../)


