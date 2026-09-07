---
title: "WorkingTimeCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkingTimeCollection method. WorkingTimeCollection ऑब्जेक्ट को WorkingTime ऑब्जेक्ट्स की सूची में परिवर्तित करता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/workingtimecollection/tolist/
---
## WorkingTimeCollection.ToList method

WorkingTimeCollection ऑब्जेक्ट को [`WorkingTime`](../../workingtime/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

```csharp
public List<WorkingTime> ToList()
```

### रिटर्न वैल्यू

[`WorkingTime`](../../workingtime/) ऑब्जेक्ट्स की सूची।

## उदाहरण

Working time संग्रह के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// शनिवार के कार्य समय को प्रिंट करें
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// रविवार के कार्य समय को प्रिंट करें
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // आप कार्य समयों के माध्यम से आगे नेविगेट कर सकते हैं और इन्हें प्रदर्शित कर सकते हैं।
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### संबंधित देखें

* class [WorkingTime](../../workingtime/)
* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


