---
title: "Asn.LinkedFields"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Καθορίζει εάν το Project είναι συνδεδεμένο με άλλο αντικείμενο OLE"
type: docs
weight: 320
url: /el/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Καθορίζει εάν το Έργο είναι συνδεδεμένο με άλλο αντικείμενο OLE.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε την ιδιότητα Asn.LinkedFields.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


