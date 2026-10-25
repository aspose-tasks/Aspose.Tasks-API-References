---
title: "Tsk.ManualDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की मैन्युअल रूप से निर्धारित अवधि को परिभाषित करता है"
type: docs
weight: 780
url: /hi/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

किसी कार्य की मैन्युअल रूप से निर्धारित अवधि को परिभाषित करता है।

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## उदाहरण

दिखाता है कि Tsk.ManualDuration प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


