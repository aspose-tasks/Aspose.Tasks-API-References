---
title: "Κλάση TaskUtils"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Util.TaskUtils. Βοηθητική κλάση που παρέχει χρήσιμες λειτουργίες με εργασίες."
type: docs
weight: 2770
url: /el/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Βοηθητική κλάση που παρέχει χρήσιμες λειτουργίες με εργασίες.

```csharp
public static class TaskUtils
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Εφαρμόζει τον καθορισμένο αλγόριθμο σε κάθε εργασία ενός δέντρου. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Βρίσκει μια εργασία που ικανοποιεί την προϋπόθεση σε ένα δέντρο εργασιών. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Υπολογίζει αναδρομικά τον αριθμό των παιδικών εργασιών μιας εργασίας σε όλα τα επίπεδα. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με έναν αλγόριθμο δέντρου.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// συλλέξτε όλες τις εργασίες του έργου
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// εργαστείτε με τις εργασίες όπως με μια απλή λίστα
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


