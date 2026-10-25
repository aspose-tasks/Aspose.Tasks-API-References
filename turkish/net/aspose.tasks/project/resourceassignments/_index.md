---
title: "Project.ResourceAssignments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. ResourceAssignmentCollection nesnesini alır"
type: docs
weight: 750
url: /tr/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

ResourceAssignmentCollection nesnesini alır.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Örnekler

Kaynak atamalarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// Yeni görev ve kaynak ekle
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Kaynağı istenen göreve atayın
project.ResourceAssignments.Add(task, resource);
```

### Ayrıca Bakınız

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


