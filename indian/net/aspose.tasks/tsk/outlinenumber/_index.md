---
title: "Tsk.OutlineNumber"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह संख्या जो कार्य की पदानुक्रमित रूपरेखा संरचना में स्थिति को दर्शाती है"
type: docs
weight: 850
url: /hi/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

संख्या जो कार्य की पदानुक्रमित रूपरेखा संरचना में स्थिति को दर्शाती है।

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
```

## उदाहरण

कार्य रूपरेखा प्रॉपर्टीज़ को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


