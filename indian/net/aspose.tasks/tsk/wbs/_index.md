---
title: "Tsk.WBS"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. कार्य विभाजन संरचना WBS कोड"
type: docs
weight: 1130
url: /hi/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

वर्क ब्रेकडाउन स्ट्रक्चर (WBS) कोड।

```csharp
public static readonly Key<string, TaskKey> WBS;
```

## उदाहरण

कार्य के WBS कोड पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


