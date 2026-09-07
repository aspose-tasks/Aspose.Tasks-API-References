---
title: "Tsk.CV"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। किसी कार्य के लिए बेसलाइन लागत और कुल लागत के बीच अंतर। लागत विचलन  लागत  बेसलाइन लागत"
type: docs
weight: 260
url: /hi/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

कार्य के लिए बेसलाइन लागत और कुल लागत के बीच का अंतर। लागत विचलन = लागत - बेसलाइन लागत

```csharp
public static readonly Key<double, TaskKey> CV;
```

## उदाहरण

दिखाता है कि कैसे कार्य लागत मान पढ़े जाएँ।

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


