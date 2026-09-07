---
title: "ResourceAssignment.ParentProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceAssignment. Λαμβάνει το γονικό έργο για αυτήν την ανάθεση"
type: docs
weight: 420
url: /el/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Λαμβάνει το γονικό έργο για αυτήν την ανάθεση.

```csharp
public Project ParentProject { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το γονικό έργο μιας ανάθεσης πόρων.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// ορίστε τη διάρκεια της ανάθεσης χρησιμοποιώντας τον προεπιλεγμένο τύπο μονάδας χρόνου του έργου.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Δείτε επίσης

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


