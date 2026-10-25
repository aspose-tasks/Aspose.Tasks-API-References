---
title: "Tsk.DurationVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की बेसलाइन अवधि और कार्य के वर्तमान अनुमानित कुल अवधि के बीच अंतर"
type: docs
weight: 320
url: /hi/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

कार्य की बेसलाइन अवधि और कुल अवधि (वर्तमान अनुमान) के बीच का अंतर।

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## उदाहरण

दिखाता है कि कैसे Tsk.DurationVariance प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


