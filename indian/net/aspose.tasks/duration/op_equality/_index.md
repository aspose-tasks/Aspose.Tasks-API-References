---
title: "Duration.op_Equality"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। यह एक मान लौटाता है जो दर्शाता है कि यह instance निर्दिष्ट object के बराबर है या नहीं।"
type: docs
weight: 140
url: /hi/net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public static bool operator ==(Duration a, Duration b)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एक | अवधि | पहला duration। |
| b | अवधि | दूसरा duration। |

### रिटर्न वैल्यू

एक मान जो दर्शाता है कि यह उदाहरण निर्दिष्ट वस्तु के बराबर है या नहीं।

## उदाहरण

duration समानता की जाँच करने का तरीका दर्शाता है।

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// duration की समानता को अंतर्निहित timespan के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


