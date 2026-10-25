---
title: "ResourceAssignment.Guid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment‑eigenschap. Haalt een unieke identifier op of stelt deze in voor deze toewijzing."
type: docs
weight: 290
url: /nl/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Geeft of stelt een unieke identifier voor deze toewijzing in.

```csharp
public Guid? Guid { get; set; }
```

## Voorbeelden

Toont hoe een resource‑toewijzing GUID te lezen.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


