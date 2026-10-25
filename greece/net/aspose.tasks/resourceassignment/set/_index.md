---
title: "ResourceAssignment.Set"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceAssignment μέθοδος. Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο"
type: docs
weight: 750
url: /el/net/aspose.tasks/resourceassignment/set/
---
## ResourceAssignment.Set&lt;T&gt; method

Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

```csharp
public void Set<T>(Key<T, AsnKey> key, T val)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | το καθορισμένο κλειδί ιδιότητας. [`Asn`](../../asn/) για λήψη του κλειδιού ιδιότητας. |
| val | η τιμή. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια ανάθεση και να λάβετε/ορίσετε κοινές ιδιότητες ανάθεσης.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


