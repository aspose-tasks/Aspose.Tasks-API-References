---
title: "Project.TaskLinks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. يحصل على كائن TaskLinkCollection."
type: docs
weight: 930
url: /ar/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

يحصل على كائن [`TaskLinkCollection`](../../tasklinkcollection/).

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## الأمثلة

يظهر كيفية إنشاء روابط المهام.

```csharp
var project = new Project();

// إضافة مهام جديدة
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// ربط المهام
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

### انظر أيضًا

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


