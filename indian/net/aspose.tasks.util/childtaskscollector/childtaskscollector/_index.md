---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ChildTasksCollector constructor. ChildTasksCollector वर्ग का नया उदाहरण आरंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

[`ChildTasksCollector`](../) वर्ग का नया उदाहरण आरंभ करता है।

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


