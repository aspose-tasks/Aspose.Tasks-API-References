---
title: "ChildTasksCollector.Tasks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ChildTasksCollector property. एकत्रित बाल वस्तु कार्यों की सूची प्राप्त करता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

एकत्रित चाइल्ड ऑब्जेक्ट्स (टास्क) की सूची प्राप्त करता है।

```csharp
public List<Task> Tasks { get; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट में सभी टास्क को एक साधारण सूची के रूप में कैसे इटरेट करें।

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


