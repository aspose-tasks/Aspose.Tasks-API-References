---
title: "WeekDay.WeekDay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WeekDay कंस्ट्रक्टर। निर्दिष्ट दिन प्रकार के साथ WeekDay क्लास का एक नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/weekday/weekday/
---
## WeekDay(DayType) {#constructor_1}

निर्दिष्ट day type के साथ [`WeekDay`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public WeekDay(DayType dayType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | DayType | निर्दिष्ट दिन प्रकार। |

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

---

## WeekDay(DayType, IEnumerable&lt;WorkingTime&gt;) {#constructor_3}

निर्दिष्ट day type और कार्य समय अवधियों की सूची के साथ [`WeekDay`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public WeekDay(DayType dayType, IEnumerable<WorkingTime> workingTimes)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | DayType | निर्दिष्ट दिन प्रकार। |
| workingTimes | IEnumerable`1 | कार्य समय अवधियों की सूची। |

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
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, params WorkingTime[]) {#constructor_2}

निर्दिष्ट day type और कार्य समय अवधियों के साथ [`WeekDay`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public WeekDay(DayType dayType, params WorkingTime[] workingTimes)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | DayType | निर्दिष्ट दिन प्रकार। |
| workingTimes | WorkingTime[] | कार्य समय अवधियों का एरे। |

### संबंधित देखें

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay() {#constructor}

[`WeekDay`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public WeekDay()
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

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


