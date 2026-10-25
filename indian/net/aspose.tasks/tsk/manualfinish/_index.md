---
title: "Tsk.ManualFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के मैन्युअल रूप से निर्धारित समाप्ति को परिभाषित करता है"
type: docs
weight: 790
url: /hi/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

किसी कार्य की मैन्युअल रूप से निर्धारित समाप्ति को परिभाषित करता है।

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## उदाहरण

दिखाता है कि Tsk.ManualFinish प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


