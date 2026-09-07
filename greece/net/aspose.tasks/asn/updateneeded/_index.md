---
title: "Asn.UpdateNeeded"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Καθορίζει αν ο πόρος που έχει εκχωρηθεί σε μια εργασία χρειάζεται ενημέρωση σχετικά με την κατάσταση της εργασίας"
type: docs
weight: 580
url: /el/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Καθορίζει εάν ο πόρος που έχει ανατεθεί σε μια εργασία χρειάζεται να ενημερωθεί σχετικά με την κατάσταση της εργασίας.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Asn.UpdateNeeded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


