---
title: "क्लास WorkingTimeCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WorkingTimeCollection क्लास। WorkingTimeCollection वस्तुओं का संग्रह दर्शाता है"
type: docs
weight: 3670
url: /hi/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

`WorkingTime` वस्तुओं का संग्रह दर्शाता है।

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | इस `WorkingTimeCollection` वस्तु में शामिल वस्तुओं की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | इस संग्रह में नया WorkingTime उदाहरण जोड़ता है। |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | संग्रह से सभी [`WorkingTime`](../workingtime/) आइटम हटाता है। |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | जाँचता है कि निर्दिष्ट तत्व सूची में है या नहीं। एक रैखिक O(n) खोज करता है। |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | एक विशिष्ट इंडेक्स से शुरू करके संग्रह की सामग्री को एक Array में कॉपी करता है |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | इस संग्रह से [`WorkingTime`](../workingtime/) उदाहरण हटाता है। |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | WorkingTimeCollection वस्तु को [`WorkingTime`](../workingtime/) वस्तुओं की सूची में परिवर्तित करता है। |

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

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


