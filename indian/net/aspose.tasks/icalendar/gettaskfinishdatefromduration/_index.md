---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ICalendar मेथड। कार्य की समाप्ति तिथि और समय की गणना उसके प्रारंभ तिथि के भागों और कार्य अवधि से करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

कार्य की प्रारंभ तिथि, विभाजित भागों और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है।

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | जिस कार्य की समाप्ति तिथि की गणना करनी है। |
| अवधि | TimeSpan | जिस अवधि की गणना करनी है। |

### रिटर्न वैल्यू

दिए गए प्रारंभ तिथि और अवधि के लिए कार्य की समाप्ति तिथि।

## टिप्पणियाँ

यदि कार्य सारांश है, null है या उसकी प्रारंभ तिथि सेट नहीं है तो DateTime.MinValue लौटाता है।

### संबंधित देखें

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


