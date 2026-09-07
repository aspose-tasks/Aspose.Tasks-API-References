---
title: "एनम DayType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DayType एनम। सप्ताह के दिन को निर्दिष्ट करता है"
type: docs
weight: 450
url: /hi/net/aspose.tasks/daytype/
---
## DayType enumeration

सप्ताह के दिन को निर्दिष्ट करता है।

```csharp
public enum DayType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Exception | `0` | Exception दिन प्रकार को दर्शाता है। |
| Sunday | `1` | Sunday दिन प्रकार को दर्शाता है। |
| Monday | `2` | Monday दिन प्रकार को दर्शाता है। |
| Tuesday | `3` | Tuesday दिन प्रकार को दर्शाता है। |
| Wednesday | `4` | Wednesday दिन प्रकार को दर्शाता है। |
| Thursday | `5` | Thursday दिन प्रकार को दर्शाता है। |
| Friday | `6` | Friday दिन प्रकार को दर्शाता है। |
| Saturday | `7` | Saturday दिन प्रकार को दर्शाता है। |

## उदाहरण

दिखाता है कि नया कैलेंडर कैसे परिभाषित करें, उसमें सप्ताह के दिन जोड़ें और दिनों के लिए कार्य समय निर्धारित करें।

```csharp
var project = new Project();

// कैलेंडर परिभाषित करें
var calendar = project.Calendars.Add("Calendar1");

// सोमवार से गुरुवार तक डिफ़ॉल्ट समय के साथ कार्य दिवस जोड़ें
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// शुक्रवार को छोटा कार्य दिवस सेट करें
var weekDay = new WeekDay(DayType.Friday);

// कार्य समय सेट करता है। केवल DateTime का समय भाग महत्वपूर्ण है।
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// प्रोजेक्ट के साथ काम कर रहे हैं...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


