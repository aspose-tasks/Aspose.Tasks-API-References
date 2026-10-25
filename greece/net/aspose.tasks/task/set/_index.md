---
title: "Task.Set"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο"
type: docs
weight: 1410
url: /el/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | Το καθορισμένο κλειδί ιδιότητας. [`Tsk`](../../tsk/) για λήψη του κλειδιού ιδιότητας. |
| val | η τιμή. |

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


