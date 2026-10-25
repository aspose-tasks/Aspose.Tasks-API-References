---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WeekDay मेथड। निर्दिष्ट सप्ताह के दिन के लिए डिफ़ॉल्ट समय अवधि सेट करता है"
type: docs
weight: 130
url: /hi/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

निर्दिष्ट सप्ताह के दिन के लिए डिफ़ॉल्ट समय अवधियों को सेट करता है।

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दिन | WeekDay | डिफ़ॉल्ट कार्य दिवस सेट करने के लिए सप्ताह का दिन। |

## उदाहरण

एक दिन के लिए डिफ़ॉल्ट कार्य समय सेट करने का तरीका दिखाता है।

```csharp
var project = new Project();

// कैलेंडर परिभाषित करें
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// सोमवार से गुरुवार तक डिफ़ॉल्ट समय के साथ कार्य दिवस जोड़ें
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// आइए सभी कार्य समय प्रिंट करें
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


