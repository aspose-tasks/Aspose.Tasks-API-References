---
title: "Project.ResourceAssignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt het ResourceAssignmentCollection-object op."
type: docs
weight: 750
url: /nl/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Haalt ResourceAssignmentCollection-object op.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Voorbeelden

Toont hoe te werken met resource-toewijzingen.

```csharp
var project = new Project();

// Nieuwe taak en resource toevoegen
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Wijs de resource de gewenste taak toe.
project.ResourceAssignments.Add(task, resource);
```

### Zie ook

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


