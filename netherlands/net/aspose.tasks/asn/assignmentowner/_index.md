---
title: "Asn.AssignmentOwner"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. De naam van een toewijzings-eigenaar"
type: docs
weight: 100
url: /nl/net/aspose.tasks/asn/assignmentowner/
---
## Asn.AssignmentOwner field

De naam van een toewijzings-eigenaar.

```csharp
public static readonly Key<string, AsnKey> AssignmentOwner;
```

## Voorbeelden

Toont hoe je de eigenschappen Asn.AssignmentOwner en Asn.AssignmentOwnerGuid kunt lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.AssignmentOwner, "Assignment Owner");
assignment.Set(Asn.AssignmentOwnerGuid, "1d440f0c-7839-4802-af5f-4bb30e8b75ab");

Console.WriteLine("Assignment Owner: " + assignment.Get(Asn.AssignmentOwner));
Console.WriteLine("Assignment Owner GUID: " + assignment.Get(Asn.AssignmentOwnerGuid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


