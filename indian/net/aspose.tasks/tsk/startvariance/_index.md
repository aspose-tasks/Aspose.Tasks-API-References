---
title: "Tsk.StartVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह समय जो कार्य या असाइनमेंट की बेसलाइन शुरू तिथि और वर्तमान निर्धारित शुरू तिथि के बीच अंतर को दर्शाता है"
type: docs
weight: 1040
url: /hi/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

समय जो कार्य या असाइनमेंट की बेसलाइन प्रारम्भ तिथि और वर्तमान में निर्धारित प्रारम्भ तिथि के बीच अंतर को दर्शाता है।

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## उदाहरण

दिखाता है कि कैसे Tsk.StartVariance प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


