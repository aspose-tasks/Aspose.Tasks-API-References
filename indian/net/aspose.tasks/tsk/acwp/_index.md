---
title: "Tsk.ACWP"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य पर अब तक किए गए काम की लागत, प्रोजेक्ट स्थिति तिथि या आज की तिथि तक"
type: docs
weight: 110
url: /hi/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

टास्क पर पहले से किए गए कार्य के लिए हुई लागत, प्रोजेक्ट स्थिति तिथि या आज की तिथि तक।

```csharp
public static readonly Key<double, TaskKey> ACWP;
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


