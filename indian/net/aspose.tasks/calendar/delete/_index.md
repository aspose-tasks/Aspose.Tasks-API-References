---
title: "Calendar.Delete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar विधि। प्रोजेक्ट से कैलेंडर को हटाता है"
type: docs
weight: 140
url: /hi/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

प्रोजेक्ट से कैलेंडर हटाता है।

```csharp
public void Delete()
```

## उदाहरण

दिखाता है कि प्रोजेक्ट से कैलेंडर कैसे हटाएँ।

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// नाम द्वारा कैलेंडर प्राप्त करें
var calendar = project.Calendars.GetByName("Broken Calendar");

// कैलेंडर को हटाएँ
calendar.Delete();
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


