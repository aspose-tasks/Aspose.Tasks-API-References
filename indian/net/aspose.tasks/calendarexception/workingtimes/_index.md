---
title: "CalendarException.WorkingTimes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException प्रॉपर्टी। WorkingTimeCollection ऑब्जेक्ट प्राप्त करता है या सेट करता है। कार्य समयों का संग्रह जो सप्ताह के दिन पर कार्य किए गए समय को परिभाषित करता है। कम से कम एक कार्य समय मौजूद होना चाहिए और अधिकतम पाँच से अधिक नहीं हो सकते।"
type: docs
weight: 160
url: /hi/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

WorkingTimeCollection ऑब्जेक्ट प्राप्त करता या सेट करता है। कार्य दिवस पर काम किए गए समय को परिभाषित करने वाले कार्य समयों का संग्रह। कम से कम एक कार्य समय मौजूद होना चाहिए, और अधिकतम पाँच से अधिक नहीं हो सकता।

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


