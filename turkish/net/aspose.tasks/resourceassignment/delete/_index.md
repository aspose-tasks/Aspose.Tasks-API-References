---
title: "ResourceAssignment.Delete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Proje atamaları koleksiyonundan kaynak atamasını siler"
type: docs
weight: 680
url: /tr/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Kaynak atamasını proje atamaları koleksiyonundan siler.

```csharp
public void Delete()
```

## Örnekler

Bir kaynak atamasının nasıl silineceğini gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Ayrıca Bakınız

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


