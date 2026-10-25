---
title: "Tsk.IsMarked"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Δείχνει εάν μια εργασία είναι σημειωμένη για περαιτέρω ενέργεια ή αναγνώριση κάποιου είδους."
type: docs
weight: 620
url: /el/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Εμφανίζει εάν μια εργασία είναι σημειωμένη για περαιτέρω ενέργεια ή κάποια μορφή ταυτοποίησης.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Παρατηρήσεις

Ισχύει μόνο για τη μορφή αρχείου mpp.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


