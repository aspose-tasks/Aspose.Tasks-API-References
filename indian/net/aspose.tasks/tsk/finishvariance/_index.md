---
title: "Tsk.FinishVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. वह समय जो कार्य या असाइनमेंट की बेसलाइन समाप्ति तिथि और उसकी वर्तमान समाप्ति तिथि के बीच अंतर दर्शाता है"
type: docs
weight: 420
url: /hi/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

कार्य या असाइनमेंट की बेसलाइन समाप्ति तिथि और उसकी वर्तमान समाप्ति तिथि के बीच के अंतर को दर्शाने वाला समय।

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## उदाहरण

दिखाता है कि कैसे Tsk.FinishVariance प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


