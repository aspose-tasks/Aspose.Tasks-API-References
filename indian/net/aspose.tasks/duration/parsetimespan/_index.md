---
title: "Duration.ParseTimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। PTHMS प्रारूप में अवधि स्ट्रिंग को पार्स करता है।"
type: docs
weight: 130
url: /hi/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

"PT--H--M--S--" प्रारूप में अवधि स्ट्रिंग को पार्स करता है।

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | स्ट्रिंग | पार्स करने के लिए निर्दिष्ट स्ट्रिंग। |

### रिटर्न वैल्यू

परिणामस्वरूप पार्स किया गया instance [`TimeSpan`](../timespan/) struct लौटाता है।

## उदाहरण

दिखाता है कि स्ट्रिंग को टाइम स्पैन में कैसे परिवर्तित किया जाए।

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


