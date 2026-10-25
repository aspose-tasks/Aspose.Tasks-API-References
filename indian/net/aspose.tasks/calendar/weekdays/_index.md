---
title: "Calendar.WeekDays"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। इस कैलेंडर के लिए WeekDaysCollection प्राप्त करता है। वह सप्ताह के दिनों का संग्रह जो कैलेंडर को परिभाषित करता है।"
type: docs
weight: 120
url: /hi/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

इस कैलेंडर के लिए WeekDaysCollection प्राप्त करता है। कैलेंडर को परिभाषित करने वाले weekdays का संग्रह।

```csharp
public WeekDayCollection WeekDays { get; }
```

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

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


