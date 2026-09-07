---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। Primavera फ़ॉर्मेट से पढ़े गए कैलेंडर के लिए Primaveraspecific प्रॉपर्टी वाला ऑब्जेक्ट प्राप्त करता है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Primavera फ़ॉर्मेट से पढ़े गए कैलेंडर के लिए Primavera-विशिष्ट गुणों वाला ऑब्जेक्ट प्राप्त करता है।

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## उदाहरण

दिखाता है कि Primavera फ़ाइल से प्रोजेक्ट कैसे पढ़ें और कैलेंडर की Primavera-विशिष्ट प्रॉपर्टी की जाँच करें।

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### संबंधित देखें

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


