---
title: "Tsk.BCWP"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की पूर्णता प्रतिशत को समय‑फेज़ बेसलाइन लागतों से गुणा करके प्राप्त संचयी मान"
type: docs
weight: 120
url: /hi/net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

टास्क के प्रतिशत पूर्णता को समय-फ़ेज़ बेसलाइन लागतों से गुणा करके प्राप्त संचयी मान।

```csharp
public static readonly Key<double, TaskKey> BCWP;
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


