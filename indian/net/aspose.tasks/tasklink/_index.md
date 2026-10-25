---
title: "क्लास TaskLink"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskLink क्लास। एक predecessor लिंक का प्रतिनिधित्व करता है"
type: docs
weight: 2410
url: /hi/net/aspose.tasks/tasklink/
---
## TaskLink class

एक पूर्ववर्ती लिंक का प्रतिनिधित्व करता है।

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | बाहरी predecessor प्रोजेक्ट को प्राप्त करता है या सेट करता है। |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | यह संकेत देने वाला मान प्राप्त करता है या सेट करता है कि क्या एक predecessor किसी अन्य प्रोजेक्ट का हिस्सा है। |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | लेग फ़ॉर्मेट को व्यक्त करने के फ़ॉर्मेट को प्राप्त करता है या सेट करता है। |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | लेग को मिनट के दशमलव हिस्से या प्रतिशत में प्राप्त करता है या सेट करता है। |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | LagFormat के आधार पर लेग अवधि को प्राप्त करता है या सेट करता है। |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | एक लिंक के प्रकार को प्राप्त करता है या सेट करता है। |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | predecessor टास्क को प्राप्त करता है या सेट करता है। |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | successor टास्क को प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | `TaskLink` क्लास के इंस्टेंस के लिए एक हैश कोड मान लौटाता है। |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | एक TaskLink की स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


