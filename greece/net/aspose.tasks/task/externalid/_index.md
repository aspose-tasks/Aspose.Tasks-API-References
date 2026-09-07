---
title: "Task.ExternalId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει ή ορίζει μια τιμή του ExternalId"
type: docs
weight: 410
url: /el/net/aspose.tasks/task/externalid/
---
## Task.ExternalId property

Λαμβάνει ή ορίζει μια τιμή του ExternalId.

```csharp
public int ExternalId { get; set; }
```

## Παραδείγματα

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


