---
title: "क्लास WeekDayCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeekDayCollection क्लास। WeekDay ऑब्जेक्ट्स का संग्रह दर्शाती है"
type: docs
weight: 3550
url: /hi/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

[`WeekDay`](../weekday/) ऑब्जेक्ट्स का संग्रह दर्शाती है।

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | `WeekDayCollection` ऑब्जेक्ट में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर आइटम मान प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | इस ऑब्जेक्ट में एक [`WeekDay`](../weekday/) इंस्टेंस जोड़ता है। |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | WeekDayCollection ऑब्जेक्ट को साफ़ करें। |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | जाँचता है कि संग्रह में निर्दिष्ट [`WeekDay`](../weekday/) है या नहीं। |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | निर्दिष्ट इंडेक्स पर संग्रह की सामग्री को एक एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | निर्दिष्ट [`WeekDay`](../weekday/) का इंडेक्स लौटाता है। |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | निर्दिष्ट इंडेक्स पर [`WeekDay`](../weekday/) सम्मिलित करता है। |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | यदि मौजूद हो तो निर्दिष्ट [`WeekDay`](../weekday/) को हटाता है। |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | निर्दिष्ट इंडेक्स पर एक आइटम हटाता है। |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | WeekDayCollection ऑब्जेक्ट को [`WeekDay`](../weekday/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

सप्ताह के दिन संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// सप्ताह के दिन साफ़ करें
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// शनिवार का सप्ताह दिन हटाएँ
calendar.WeekDays.RemoveAt(5);

// रविवार का सप्ताह दिन हटाएँ
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// सप्ताह के दिन कॉपी करें
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### संबंधित देखें

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


