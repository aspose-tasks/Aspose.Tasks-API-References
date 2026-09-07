---
title: "Tsk.IsEffortDriven"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि कार्य की समय-सारणी प्रयास-आधारित है या नहीं"
type: docs
weight: 570
url: /hi/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

निर्धारित करता है कि कार्य का शेड्यूलिंग प्रयास-आधारित शेड्यूलिंग है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
```

## उदाहरण

दिखाता है कि महत्वपूर्ण और/या प्रयास-आधारित कार्यों को कैसे खोजें।

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


