---
title: "क्लास WeekDay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeekDay क्लास। एक सप्ताह के कार्यदिवस को दर्शाता है जो या तो सप्ताह के नियमित दिनों या कैलेंडर में अपवाद दिनों को परिभाषित करता है।"
type: docs
weight: 3540
url: /hi/net/aspose.tasks/weekday/
---
## WeekDay class

एक सप्ताह का दिन दर्शाता है जो या तो सप्ताह के नियमित दिनों को या कैलेंडर में अपवाद दिनों को परिभाषित करता है।

```csharp
public class WeekDay
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WeekDay](weekday/#constructor)() | `WeekDay` क्लास का नया उदाहरण प्रारंभ करता है। |
| [WeekDay](weekday/#constructor_1)(DayType) | निर्दिष्ट दिन प्रकार के साथ `WeekDay` क्लास का नया उदाहरण प्रारंभ करता है। |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | निर्दिष्ट दिन प्रकार और कार्य समय अवधि की सूची के साथ `WeekDay` क्लास का नया उदाहरण प्रारंभ करता है। |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | निर्दिष्ट दिन प्रकार और कार्य समय अवधियों के साथ `WeekDay` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | एक दिन का प्रकार प्राप्त करता है। |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | एक अपवाद समय की शुरुआत को प्राप्त करता है या सेट करता है। |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | एक अपवाद समय का अंत प्राप्त करता है या सेट करता है। |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | इस WeekDay उदाहरण के लिए WorkingTimeCollection प्राप्त करता है। कार्य समयों का संग्रह जो सप्ताह के कार्यदिवस पर काम किए गए समय को परिभाषित करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | डिफ़ॉल्ट कार्य दिवस बनाता है। |
| [Clone](../../aspose.tasks/weekday/clone/)() | सप्ताह के दिन की गहरी प्रतिलिपि लौटाता है। |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | `WeekDay` क्लास के उदाहरण के लिए हैश कोड मान लौटाता है। |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | सप्ताह के दिन के लिए कार्य समय लौटाता है। |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | .Net के DayOfWeek को [`DayType`](./daytype/) में कास्ट करता है। |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | निर्दिष्ट सप्ताह के दिन के लिए डिफ़ॉल्ट समय अवधियों को सेट करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


