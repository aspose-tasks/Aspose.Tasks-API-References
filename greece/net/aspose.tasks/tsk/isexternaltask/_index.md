---
title: "Tsk.IsExternalTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Καθορίζει εάν μια εργασία είναι εξωτερική"
type: docs
weight: 600
url: /el/net/aspose.tasks/tsk/isexternaltask/
---
## Tsk.IsExternalTask field

Καθορίζει εάν μια εργασία είναι εξωτερική.

```csharp
public static readonly Key<bool, TaskKey> IsExternalTask;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsExternalTask.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExternalTask, true);

Console.WriteLine("Is External Task: " + task.Get(Tsk.IsExternalTask));
```

Δείχνει πώς να δημιουργήσετε σύνδεσμο εργασίας δια-έργου - σύνδεσμο προς εργασία σε άλλο (εξωτερικό) έργο.

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Για να δημιουργήσουμε σύνδεσμο προς εργασία από άλλο έργο, πρέπει να δημιουργήσουμε
// το αντίγραφό της (ή "εξωτερική") εργασία στο τρέχον έργο.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


