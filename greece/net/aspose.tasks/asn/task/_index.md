---
title: "Asn.Task"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η εργασία στην οποία εκχωρείται ένας πόρος"
type: docs
weight: 550
url: /el/net/aspose.tasks/asn/task/
---
## Asn.Task field

Η εργασία στην οποία έχει ανατεθεί ένας πόρος.

```csharp
public static readonly Key<Task, AsnKey> Task;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ιδιότητες Asn.Task και Asn.Resource.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Task](../../task/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


