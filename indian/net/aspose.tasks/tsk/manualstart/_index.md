---
title: "Tsk.ManualStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। किसी कार्य की मैन्युअल रूप से निर्धारित प्रारंभ को परिभाषित करता है"
type: docs
weight: 800
url: /hi/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

किसी कार्य की मैन्युअल रूप से निर्धारित शुरुआत को परिभाषित करता है।

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## उदाहरण

दिखाता है कि कैसे Tsk.ManualStart प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


