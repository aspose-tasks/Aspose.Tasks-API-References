---
title: "TaskLink.PredTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLink प्रॉपर्टी। पूर्ववर्ती कार्य को प्राप्त करता है या सेट करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

predecessor टास्क को प्राप्त करता है या सेट करता है।

```csharp
public Task PredTask { get; set; }
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

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


