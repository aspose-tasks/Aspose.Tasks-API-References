---
title: "Project.GetPredecessors"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। निर्दिष्ट टास्क के पूर्ववर्ती होने वाले टास्क लिंक का संग्रह लौटाता है।"
type: docs
weight: 1120
url: /hi/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

निर्दिष्ट टास्क के पूर्ववर्ती टास्क लिंक का संग्रह लौटाता है।

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | वह टास्क जिसके लिए पूर्ववर्ती प्राप्त करने हैं। |

### रिटर्न वैल्यू

पूर्ववर्ती [`TaskLink`](../../tasklink/) की सूची।

## उदाहरण

विशिष्ट टास्क के लिए पूर्ववर्ती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// predecessor और successor टास्क के नाम प्रदर्शित करें
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


