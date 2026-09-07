---
title: "Tsk.RemainingDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के अधूरे भाग को पूरा करने के लिए आवश्यक समय"
type: docs
weight: 960
url: /hi/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

कार्य के अधूरे भाग को पूरा करने के लिए आवश्यक समय।

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## उदाहरण

Tsk.RemainingDuration प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


