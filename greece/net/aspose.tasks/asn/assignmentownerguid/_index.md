---
title: "Asn.AssignmentOwnerGuid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Ο παγκοσμίως μοναδικός αναγνωριστικός αριθμός ενός ιδιοκτήτη ανάθεσης"
type: docs
weight: 110
url: /el/net/aspose.tasks/asn/assignmentownerguid/
---
## Asn.AssignmentOwnerGuid field

Το παγκοσμίως μοναδικό αναγνωριστικό του ιδιοκτήτη μιας ανάθεσης.

```csharp
public static readonly Key<string, AsnKey> AssignmentOwnerGuid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες Asn.AssignmentOwner και Asn.AssignmentOwnerGuid.

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

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


