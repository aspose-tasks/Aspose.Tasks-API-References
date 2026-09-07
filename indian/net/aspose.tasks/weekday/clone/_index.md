---
title: "WeekDay.Clone"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WeekDay मेथड। सप्ताह के दिन की एक डीप कॉपी लौटाता है।"
type: docs
weight: 80
url: /hi/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

सप्ताह के दिन की गहरी प्रतिलिपि लौटाता है।

```csharp
public WeekDay Clone()
```

### रिटर्न वैल्यू

सप्ताह के दिन की डीप कॉपी लौटाता है।

## उदाहरण

दिखाता है कि सप्ताह के दिन को कैसे क्लोन किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// सप्ताह के दिन की डीप कॉपी बनाएं
var weekDay2 = weekDay1.Clone();

// कैलेंडरों की समानता को सप्ताह के दिन की प्रॉपर्टीज़ के विरुद्ध जांचा जाता है:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### संबंधित देखें

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


