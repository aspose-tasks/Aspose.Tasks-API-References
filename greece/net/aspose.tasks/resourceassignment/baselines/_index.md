---
title: "ResourceAssignment.Baselines"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceAssignment. Λαμβάνει το αντικείμενο AssignmentBaselineCollection. Η συλλογή των τιμών βάσης που σχετίζονται με μια εκχώρηση"
type: docs
weight: 120
url: /el/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Λαμβάνει το αντικείμενο AssignmentBaselineCollection. Η συλλογή των τιμών βάσης που σχετίζονται με μια ανάθεση.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Παραδείγματα

Δείχνει πώς να αποκτήσετε πρόσβαση στις βάσεις της εκχώρησης.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### Δείτε επίσης

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


