---
title: "TaskLink.LagFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLink प्रॉपर्टी। लैग फ़ॉर्मेट को व्यक्त करने के लिए फ़ॉर्मेट को प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

लेग फ़ॉर्मेट को व्यक्त करने के फ़ॉर्मेट को प्राप्त करता है या सेट करता है।

```csharp
public TimeUnitType LagFormat { get; set; }
```

## उदाहरण

प्रोजेक्ट टास्क लिंक को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// predecessor और successor टास्क के नाम प्रदर्शित करें
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### संबंधित देखें

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


