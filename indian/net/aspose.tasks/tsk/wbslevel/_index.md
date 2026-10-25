---
title: "Tsk.WBSLevel"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. कार्य का सबसे दायाँ WBS स्तर"
type: docs
weight: 1140
url: /hi/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

कार्य का सबसे दायां WBS स्तर।

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
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


