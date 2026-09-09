---
title: "ResourceAssignment.ParentProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment özelliği. Bu atama için üst proje alır"
type: docs
weight: 420
url: /tr/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Bu atama için üst proje alır.

```csharp
public Project ParentProject { get; }
```

## Örnekler

Bir kaynak atamasının üst projesinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// Varsayılan proje zaman birimi türünü kullanarak atamanın süresini ayarla.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Ayrıca Bakınız

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


