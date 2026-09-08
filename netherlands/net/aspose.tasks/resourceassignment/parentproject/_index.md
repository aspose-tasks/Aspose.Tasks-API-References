---
title: "ResourceAssignment.ParentProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-eigenschap. Haalt het bovenliggende project op voor deze toewijzing"
type: docs
weight: 420
url: /nl/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Haalt het bovenliggende project voor deze toewijzing op.

```csharp
public Project ParentProject { get; }
```

## Voorbeelden

Toont hoe het bovenliggende project van een resource‑toewijzing te gebruiken.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// stel een duur van de toewijzing in door het standaard projecttijdseenheidstype te gebruiken.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Zie ook

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


