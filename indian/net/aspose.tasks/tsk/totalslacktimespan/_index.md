---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह समय जिसमें कार्य की समाप्ति तिथि को परियोजना की समाप्ति तिथि को विलंबित किए बिना विलंबित किया जा सकता है"
type: docs
weight: 1090
url: /hi/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

कार्य की समाप्ति तिथि को परियोजना की समाप्ति तिथि को देर किए बिना विलंबित किया जा सकने वाला समय।

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## उदाहरण

दिखाता है कि कैसे Tsk.TotalSlackTimeSpan प्रॉपर्टी को पढ़ें। यह प्रॉपर्टी गणना की गई है, इसलिए आमतौर पर इसे स्पष्ट रूप से सेट करने की आवश्यकता नहीं होती।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


