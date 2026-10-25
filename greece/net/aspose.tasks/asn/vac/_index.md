---
title: "Asn.VAC"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η διαφορά μεταξύ του κόστους βάσης και του συνολικού κόστους"
type: docs
weight: 590
url: /el/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

Η διαφορά μεταξύ του βασικού κόστους και του συνολικού κόστους.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε την ιδιότητα Asn.VAC.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


