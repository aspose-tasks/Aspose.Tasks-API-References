---
title: "WeekDay.DayType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WeekDay प्रॉपर्टी. एक दिन के प्रकार को प्राप्त करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/weekday/daytype/
---
## WeekDay.DayType property

एक दिन का प्रकार प्राप्त करता है।

```csharp
public DayType DayType { get; }
```

## उदाहरण

सप्ताह के दिनों को परिभाषित करके नया कैलेंडर बनाने का तरीका दर्शाता है।

```csharp
var project = new Project();

// कैलेंडर परिभाषित करें
var calendar = project.Calendars.Add("Calendar1");

// सोमवार से गुरुवार तक डिफ़ॉल्ट समय के साथ कार्य दिवस जोड़ें
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// अपवाद दिन की प्रारंभ और समाप्ति तिथियों की जाँच करें
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// शुक्रवार को छोटा कार्य दिवस सेट करें

// कार्य समय सेट करता है। 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// <see cref="DayOfWeek" /> को <see cref="Aspose.Tasks.DayType" /> में परिवर्तित करने का एक तरीका है।
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


