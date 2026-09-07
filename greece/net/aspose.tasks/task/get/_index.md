---
title: "Task.Get"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Επιστρέφει την τιμή στην οποία αντιστοιχεί η ιδιότητα σε αυτό το κοντέινερ"
type: docs
weight: 1340
url: /el/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | Το καθορισμένο κλειδί ιδιότητας. [`Tsk`](../../tsk/) για λήψη του κλειδιού ιδιότητας. |

### Τιμή Επιστροφής

η τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

## Παραδείγματα

Δείχνει πώς να λαμβάνετε/ορίζετε ιδιότητες εργασίας.

```csharp
var project = new Project();

// Προσθέστε εργασία και ορίστε τις ιδιότητες της εργασίας
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


