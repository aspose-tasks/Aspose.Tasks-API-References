---
title: "Project.TaskLinks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। TaskLinkCollection ऑब्जेक्ट प्राप्त करता है"
type: docs
weight: 930
url: /hi/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

[`TaskLinkCollection`](../../tasklinkcollection/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## उदाहरण

टास्क लिंक बनाने का तरीका दर्शाता है।

```csharp
var project = new Project();

// नए कार्य जोड़ें।
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// टास्क को लिंक करें
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### संबंधित देखें

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


