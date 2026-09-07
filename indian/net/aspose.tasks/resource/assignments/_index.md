---
title: "Resource.Assignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी। इस ऑब्जेक्ट के लिए रिसोर्स असाइनमेंट्स का संग्रह प्राप्त करता है"
type: docs
weight: 120
url: /hi/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

इस ऑब्जेक्ट के लिए संसाधन असाइनमेंट्स का संग्रह प्राप्त करता है।

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## उदाहरण

रिसोर्स के असाइनमेंट पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### संबंधित देखें

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


