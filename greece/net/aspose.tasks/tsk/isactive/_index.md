---
title: "Tsk.IsActive"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Καθορίζει εάν μια εργασία είναι ενεργή. Οι ανενεργές εργασίες δεν επηρεάζουν πλέον άλλες εργασίες ή το συνολικό χρονοδιάγραμμα του Project"
type: docs
weight: 550
url: /el/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Καθορίζει εάν μια εργασία είναι ενεργή. Οι ανενεργές εργασίες δεν επηρεάζουν πλέον άλλες εργασίες ή το συνολικό πρόγραμμα του Project.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


