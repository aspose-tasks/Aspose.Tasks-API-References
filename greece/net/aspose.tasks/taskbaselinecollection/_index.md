---
title: "Κλάση TaskBaselineCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TaskBaselineCollection. Αναπαριστά μια συλλογή αντικειμένων TaskBaseline"
type: docs
weight: 2380
url: /el/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Αναπαριστά μια συλλογή αντικειμένων [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο TaskBaselineCollection. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Αυτή είναι η ψευδοεφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Αφαιρεί το baseline από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Μετατρέπει το αντικείμενο TaskBaselineCollection σε λίστα αντικειμένων [`TaskBaseline`](../taskbaseline/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές baseline εργασιών.

```csharp
var project = new Project();

// δημιουργήστε baseline έργου
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// εκτυπώστε baseline εργασιών
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// ας καθαρίσουμε όλα τα baseline
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Δείτε επίσης

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


