---
title: "CalendarCollection.Remove"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection मेथड। प्रोजेक्ट CalendarCollection से कैलेंडर को हटाता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

प्रोजेक्ट CalendarCollection से कैलेंडर हटाता है।

```csharp
public bool Remove(Calendar item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आइटम | कैलेंडर | हटाने के लिए कैलेंडर। |

### रिटर्न वैल्यू

यदि हटाया गया तो true लौटाता है, अन्यथा false लौटाता है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | जब कैलेंडर को हटाया नहीं जा सकता तो थ्रो किया जाता है। |

## उदाहरण

कलेक्शन में कैलेंडर को बदलने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// नया कैलेंडर जोड़ें
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


