---
title: "Tsk.WorkVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के बेसलाइन कार्य और वर्तमान में नियोजित कार्य के बीच का अंतर"
type: docs
weight: 1160
url: /hi/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

कार्य के बेसलाइन कार्य और वर्तमान में निर्धारित कार्य के बीच अंतर।

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## उदाहरण

Tsk.WorkVariance प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


