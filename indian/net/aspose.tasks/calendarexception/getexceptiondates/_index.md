---
title: "CalendarException.GetExceptionDates"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException मेथड। उन तिथियों को लौटाता है जिन पर कैलेंडर अपवाद लागू होता है"
type: docs
weight: 190
url: /hi/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

उन तिथियों को लौटाता है जिन पर कैलेंडर अपवाद लागू होता है।

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### रिटर्न वैल्यू

कैलेंडर अपवाद के लागू होने वाली अपवाद तिथियों का एक संग्रह लौटाता है।

## उदाहरण

दिखाता है कि कैसे उन तिथियों को प्राप्त किया जाए जिन पर एक विशिष्ट कैलेंडर अपवाद प्रभावी है।

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### संबंधित देखें

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


