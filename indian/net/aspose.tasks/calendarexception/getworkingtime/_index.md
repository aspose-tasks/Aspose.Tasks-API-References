---
title: "CalendarException.GetWorkingTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException मेथड। कैलेंडर अपवाद के लिए कार्य समय लौटाता है।"
type: docs
weight: 200
url: /hi/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

कैलेंडर अपवाद के लिए कार्य समय लौटाता है।

```csharp
public TimeSpan GetWorkingTime()
```

### रिटर्न वैल्यू

इस कैलेंडर अपवाद के लिए कार्य समय लौटाता है।

## उदाहरण

कैलेंडर अपवाद का कार्य समय कैसे प्राप्त करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### संबंधित देखें

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


