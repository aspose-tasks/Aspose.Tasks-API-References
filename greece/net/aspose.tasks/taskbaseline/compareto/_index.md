---
title: "TaskBaseline.CompareTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskBaseline. Υλοποίηση της διεπαφής IComparable. Συγκρίνει αυτήν την παρουσία με το καθορισμένο αντικείμενο Baseline"
type: docs
weight: 90
url: /el/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

Υλοποίηση της διεπαφής IComparable. Συγκρίνει αυτήν την παρουσία με το καθορισμένο αντικείμενο Baseline.

```csharp
public int CompareTo(TaskBaseline other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | TaskBaseline | το καθορισμένο αντικείμενο Baseline για σύγκριση με αυτήν την περίπτωση. |

### Τιμή Επιστροφής

επιστρέφει -1 εάν αυτή η περίπτωση είναι μικρότερη από το καθορισμένο αντικείμενο, 1 εάν αυτή η περίπτωση είναι μεγαλύτερη από το καθορισμένο αντικείμενο· διαφορετικά επιστρέφει 0.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των baselines.

```csharp
var project = new Project();

// Δημιουργία TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Εμφάνιση διάρκειας baseline εργασίας
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// Η ισότητα των baselines ελέγχεται σε σχέση με τους αριθμούς του baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Δείτε επίσης

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


