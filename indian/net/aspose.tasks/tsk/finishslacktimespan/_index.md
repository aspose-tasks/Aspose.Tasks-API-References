---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. प्रारंभिक समाप्ति और अंतिम समाप्ति तिथियों के बीच की अवधि।"
type: docs
weight: 400
url: /hi/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

प्रारंभिक समाप्ति और अंतिम समाप्ति तिथियों के बीच की अवधि।

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## उदाहरण

Tsk.FinishSlackTimeSpan प्रॉपर्टी को पढ़ने का तरीका दिखाता है। यह प्रॉपर्टी गणना की गई है, इसलिए आमतौर पर इसे स्पष्ट रूप से सेट करने की आवश्यकता नहीं होती।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


