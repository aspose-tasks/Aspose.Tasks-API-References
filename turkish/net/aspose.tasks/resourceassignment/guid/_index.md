---
title: "ResourceAssignment.Guid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment özelliği. Bu atama için benzersiz tanımlayıcıyı alır veya ayarlar"
type: docs
weight: 290
url: /tr/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Bu atama için benzersiz tanımlayıcıyı alır veya ayarlar.

```csharp
public Guid? Guid { get; set; }
```

## Örnekler

Bir kaynak atama GUID'sinin nasıl okunacağını gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Ayrıca Bakınız

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


