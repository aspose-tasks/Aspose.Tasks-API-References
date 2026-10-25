---
title: "ResourceAssignment.ToString"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। ResourceAssignment क्लास की इंस्टेंस का छोटा स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं।"
type: docs
weight: 790
url: /hi/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

[`ResourceAssignment`](../) क्लास की इंस्टेंस का छोटा स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं।

```csharp
public override string ToString()
```

### रिटर्न वैल्यू

छोटा स्ट्रिंग जो असाइनमेंट ऑब्जेक्ट का प्रतिनिधित्व करता है।

## उदाहरण

सामान्य असाइनमेंट जानकारी को प्रिंट करने का तरीका दिखाता है।

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


