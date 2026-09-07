---
title: "ResourceAssignment.Delete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceAssignment μέθοδος. Διαγράφει την ανάθεση πόρων από τη συλλογή αναθέσεων έργου"
type: docs
weight: 680
url: /el/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Διαγράφει την ανάθεση πόρων από τη συλλογή αναθέσεων έργου.

```csharp
public void Delete()
```

## Παραδείγματα

Δείχνει πώς να διαγράψετε μια ανάθεση πόρων.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Δείτε επίσης

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


