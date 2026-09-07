---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह समय जिसमें कार्य को किसी भी उत्तराधिकारी कार्य को विलंबित किए बिना विलंबित किया जा सकता है"
type: docs
weight: 450
url: /hi/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

ऐसा समय जिसमें कार्य को विलंबित किया जा सकता है बिना किसी उत्तराधिकारी कार्य को विलंबित किए।

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## उदाहरण

दिखाता है कि कैसे Tsk.FreeSlackTimeSpan प्रॉपर्टी को पढ़ें। यह प्रॉपर्टी गणना की गई है, इसलिए आमतौर पर इसे स्पष्ट रूप से सेट करने की आवश्यकता नहीं होती।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


