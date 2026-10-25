---
title: "Asn.Cost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Το προβλεπόμενο ή προγραμματισμένο κόστος μιας ανάθεσης"
type: docs
weight: 180
url: /el/net/aspose.tasks/asn/cost/
---
## Asn.Cost field

Το προβλεπόμενο ή προγραμματισμένο κόστος μιας ανάθεσης.

```csharp
public static readonly Key<decimal, AsnKey> Cost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες του πραγματικού κόστους.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
assignment.Set(Asn.Cost, 10);
assignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));
assignment.Set(Asn.ActualStart, new DateTime(2000, 1, 3, 8, 0, 0));
assignment.Set(Asn.ActualCost, 10m);
assignment.Set(Asn.ActualFinish, new DateTime(2000, 1, 3, 17, 0, 0));

Console.WriteLine("Start: " + assignment.Get(Asn.Start));
Console.WriteLine("Cost: " + assignment.Get(Asn.Cost));
Console.WriteLine("Finish: " + assignment.Get(Asn.Finish));
Console.WriteLine("Actual Start: " + assignment.Get(Asn.ActualStart));
Console.WriteLine("Actual Cost: " + assignment.Get(Asn.ActualCost));
Console.WriteLine("Actual Finish: " + assignment.Get(Asn.ActualFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


