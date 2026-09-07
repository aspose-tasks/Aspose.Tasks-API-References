---
title: "Tsk.SubprojectName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η πηγαία θέση ενός υποέργου"
type: docs
weight: 1070
url: /el/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

Η πηγή τοποθεσίας ενός υποέργου.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια εργασία υποέργου.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Προσθήκη εργασίας
var task = project.RootTask.Children.Add("Task 1");

// Ορισμός νέου συνδέσμου υποέργου
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


