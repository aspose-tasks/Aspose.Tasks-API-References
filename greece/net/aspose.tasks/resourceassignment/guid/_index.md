---
title: "ResourceAssignment.Guid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceAssignment. Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό για αυτήν την ανάθεση."
type: docs
weight: 290
url: /el/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό για αυτήν την ανάθεση.

```csharp
public Guid? Guid { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα GUID ανάθεσης πόρου.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Δείτε επίσης

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


