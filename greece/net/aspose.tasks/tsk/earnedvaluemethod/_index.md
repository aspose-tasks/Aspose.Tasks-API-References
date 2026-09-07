---
title: "Tsk.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν πρέπει να χρησιμοποιηθεί το πεδίο Complete ή Physical Complete για τον υπολογισμό του προϋπολογισμένου κόστους του εκτελεσθέντος έργου (BCWP)"
type: docs
weight: 350
url: /el/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Καθορίζει εάν το πεδίο % Complete ή Physical % Complete πρέπει να χρησιμοποιηθεί για τον υπολογισμό του προϋπολογισμένου κόστους της εκτελεσθείσας εργασίας (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.EarnedValueMethod.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


