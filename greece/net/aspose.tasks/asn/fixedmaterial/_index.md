---
title: "Asn.FixedMaterial"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn field. Καθορίζει αν η κατανάλωση ενός ανατεθειμένου υλικού πόρου συμβαίνει σε ένα ενιαίο σταθερό ποσό"
type: docs
weight: 260
url: /el/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Καθορίζει εάν η κατανάλωση ενός ανατεθειμένου υλικού πόρου συμβαίνει σε ένα ενιαίο, σταθερό ποσό.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Asn.FixedMaterial.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


