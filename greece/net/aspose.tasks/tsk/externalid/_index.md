---
title: "Tsk.ExternalId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Εάν μια εργασία είναι εξωτερική, περιέχει το εξωτερικό Id της εργασίας"
type: docs
weight: 360
url: /el/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

Εάν μια εργασία είναι εξωτερική, περιέχει το εξωτερικό Id της εργασίας.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## Παραδείγματα

Δείχνει πώς να εντοπίσετε εργασίες δια-έργου.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// Εμφανίστε το ID της εργασίας στο εξωτερικό έργο
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// Εμφανίστε το ID της εργασίας στο αρχικό έργο
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
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


