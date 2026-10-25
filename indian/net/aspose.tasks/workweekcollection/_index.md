---
title: "क्लास WorkWeekCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WorkWeekCollection क्लास। WorkWeek ऑब्जेक्ट्स का संग्रह दर्शाता है।"
type: docs
weight: 3650
url: /hi/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

[`WorkWeek`](../workweek/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | इस `WorkWeekCollection` ऑब्जेक्ट में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | पैरेंट कैलेंडर प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | इस संग्रह ऑब्जेक्ट में WorkWeek इंस्टेंस जोड़ता है। |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | WorkWeekCollection ऑब्जेक्ट को [`WorkWeek`](../workweek/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


