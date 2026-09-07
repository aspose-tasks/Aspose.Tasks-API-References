---
title: "Project.ResourceAssignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο ResourceAssignmentCollection"
type: docs
weight: 750
url: /el/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Λαμβάνει το αντικείμενο ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις αναθέσεις πόρων.

```csharp
var project = new Project();

// Προσθήκη νέας εργασίας και πόρου
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Αναθέστε το επιθυμητό έργο στον πόρο
project.ResourceAssignments.Add(task, resource);
```

### Δείτε επίσης

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


