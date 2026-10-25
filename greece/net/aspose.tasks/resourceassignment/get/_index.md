---
title: "ResourceAssignment.Get"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceAssignment μέθοδος. Επιστρέφει την τιμή στην οποία αντιστοιχεί η ιδιότητα σε αυτό το κοντέινερ"
type: docs
weight: 700
url: /el/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | το καθορισμένο κλειδί ιδιότητας. [`Asn`](../../asn/) για λήψη του κλειδιού ιδιότητας. |

### Τιμή Επιστροφής

η τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

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


