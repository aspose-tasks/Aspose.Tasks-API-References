---
title: "ResourceAssignment.ToString"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceAssignment μέθοδος. Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς της παρουσίας της κλάσης ResourceAssignment. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν"
type: docs
weight: 790
url: /el/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς της παρουσίας της κλάσης [`ResourceAssignment`](../). Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν.

```csharp
public override string ToString()
```

### Τιμή Επιστροφής

σύντομη συμβολοσειρά που αντιπροσωπεύει το αντικείμενο ανάθεσης.

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε κοινές πληροφορίες ανάθεσης.

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


