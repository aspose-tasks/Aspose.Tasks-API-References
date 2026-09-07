---
title: "Calendar.Exceptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। CalendarExceptionCollection ऑब्जेक्ट प्राप्त करता है। वह अपवादों का संग्रह जो कैलेंडर से जुड़ा है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

CalendarExceptionCollection ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी अपवादों का संग्रह।

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## उदाहरण

कैलेंडर अपवादों के बारे में जानकारी प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// कैलेंडरों पर इटररेट करें
foreach (var calendar in project.Calendars)
{
    // कैलेंडर अपवादों तक पहुँचें
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### संबंधित देखें

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


