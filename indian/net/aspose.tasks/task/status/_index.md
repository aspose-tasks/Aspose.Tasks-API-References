---
title: "Task.Status"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। कार्य की स्थिति प्राप्त करता है।"
type: docs
weight: 1160
url: /hi/net/aspose.tasks/task/status/
---
## Task.Status property

टास्क की स्थिति प्राप्त करता है।

```csharp
public TaskStatus Status { get; }
```

## उदाहरण

कार्य की स्थिति प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// प्रोजेक्ट की स्टेटस डेट सेट की जानी चाहिए क्योंकि स्टेटस कैलकुलेशन स्टेटस डेट का उपयोग करता है।
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### संबंधित देखें

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


