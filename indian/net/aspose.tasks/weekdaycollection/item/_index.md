---
title: "WeekDayCollection.Item"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WeekDayCollection प्रॉपर्टी। निर्दिष्ट इंडेक्स पर आइटम मान को प्राप्त करता है या सेट करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/weekdaycollection/item/
---
## WeekDayCollection indexer

निर्दिष्ट इंडेक्स पर आइटम मान प्राप्त करता है या सेट करता है।

```csharp
public WeekDay this[int index] { get; set; }
```

| पैरामीटर | विवरण |
| --- | --- |
| इंडेक्स | प्राप्त या सेट करने वाले तत्व का शून्य-आधारित अनुक्रमणिका। |

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

* class [WeekDay](../../weekday/)
* class [WeekDayCollection](../)
* namespace [Aspose.Tasks](../../weekdaycollection/)
* assembly [Aspose.Tasks](../../../)


