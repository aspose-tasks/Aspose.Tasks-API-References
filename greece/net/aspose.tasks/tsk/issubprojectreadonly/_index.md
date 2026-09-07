---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Καθορίζει αν ένα υποπρόγραμμα είναι μόνο για ανάγνωση."
type: docs
weight: 710
url: /el/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

Καθορίζει εάν ένα υποέργο είναι μόνο για ανάγνωση.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsSubprojectReadOnly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


