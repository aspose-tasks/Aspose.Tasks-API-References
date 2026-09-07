---
title: "Task.Assignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी. प्राप्त करता है इस ऑब्जेक्ट के लिए रिसोर्स असाइनमेंट्स का संग्रह"
type: docs
weight: 120
url: /hi/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

इस ऑब्जेक्ट के लिए संसाधन असाइनमेंट्स का संग्रह प्राप्त करता है।

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## उदाहरण

दिखाता है कि टास्क के असाइनमेंट्स पर कैसे इटरेट किया जाए।

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // टास्क के असाइनमेंट प्रदर्शित करें
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### संबंधित देखें

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


