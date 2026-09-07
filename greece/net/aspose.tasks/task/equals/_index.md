---
title: "Task.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη εργασία"
type: docs
weight: 1330
url: /el/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια συγκεκριμένη εργασία.

```csharp
public bool Equals(Task other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | Εργασία | Η καθορισμένη εργασία για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

επιστρέφει true εάν η καθορισμένη εργασία και αυτή η παρουσία έχουν ίδιες μοναδικές ταυτότητες.

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τις αναθέσεις της εργασίας.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // εμφάνιση των αναθέσεων της εργασίας
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Το καθορισμένο αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

επιστρέφει true εάν η καθορισμένη εργασία και αυτή η παρουσία έχουν ίδιες μοναδικές ταυτότητες.

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τις αναθέσεις της εργασίας.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // εμφάνιση των αναθέσεων της εργασίας
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


