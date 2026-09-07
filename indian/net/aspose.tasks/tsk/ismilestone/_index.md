---
title: "Tsk.IsMilestone"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। यह निर्धारित करता है कि कार्य एक माइलस्टोन है या नहीं"
type: docs
weight: 630
url: /hi/net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

निर्धारित करता है कि कार्य एक माइलस्टोन है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
```

## उदाहरण

दिखाता है कि अनुमानित और/या माइलस्टोन कार्यों को कैसे खोजें।

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// संग्रहित कार्यों पर इटरेट करें
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


