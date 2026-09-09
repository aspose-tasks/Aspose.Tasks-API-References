---
title: "Project.TaskLinks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. TaskLinkCollection nesnesini alır"
type: docs
weight: 930
url: /tr/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

[`TaskLinkCollection`](../../tasklinkcollection/) nesnesini alır.

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Örnekler

Görev bağlantılarının nasıl oluşturulacağını gösterir.

```csharp
var project = new Project();

// Yeni görevler ekle
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Görevleri bağlayın
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

### Ayrıca Bakınız

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


