---
title: "Calendar.IsBaselineCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि कैलेंडर बेसलाइन कैलेंडर है या नहीं"
type: docs
weight: 80
url: /hi/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

कैलेंडर बेसलाइन कैलेंडर है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool IsBaselineCalendar { get; set; }
```

## उदाहरण

दिखाता है कि कैलेंडर बेसलाइन कैलेंडर है या नहीं, कैसे जांचें।

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


