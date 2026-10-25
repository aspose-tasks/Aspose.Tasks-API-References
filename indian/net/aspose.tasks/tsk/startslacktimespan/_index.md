---
title: "Tsk.StartSlackTimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। प्रारंभिक शुरू और देर से शुरू तिथियों के बीच की अवधि"
type: docs
weight: 1020
url: /hi/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

प्रारंभिक प्रारम्भ और देर से प्रारम्भ तिथियों के बीच की अवधि।

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## उदाहरण

दिखाता है कि Tsk.StartSlackTimeSpan प्रॉपर्टी को कैसे पढ़ें। यह प्रॉपर्टी गणना की जाती है, इसलिए आमतौर पर इसे स्पष्ट रूप से सेट करने की आवश्यकता नहीं होती।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


