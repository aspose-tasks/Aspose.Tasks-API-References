---
title: "Tsk.ActivityId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Αντιπροσωπεύει το πεδίο activity id, ένα μοναδικό αναγνωριστικό εργασίας που χρησιμοποιείται από το Primavera. Ισχύει μόνο για έργα Primavera"
type: docs
weight: 10
url: /el/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Αναπαριστά το πεδίο id δραστηριότητας - το μοναδικό αναγνωριστικό ενός έργου που χρησιμοποιείται από το Primavera. (εφαρμόζεται μόνο σε έργα Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με το πεδίο ActivityId ειδικό για έργα Primavera

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Δημιουργήστε επιλογές αποθήκευσης Primavera και καθορίστε ότι τα ActivityIds δεν πρέπει να αντικατασταθούν κατά την αποθήκευση.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


