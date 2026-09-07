---
title: "TaskBaseline.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskBaseline method. Επιστρέφει μια τιμή που υποδεικνύει αν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline"
type: docs
weight: 100
url: /el/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline.

```csharp
public bool Equals(TaskBaseline other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | TaskBaseline | το καθορισμένο αντικείμενο AssignmentBaseline για σύγκριση με αυτήν την παρουσίαση. |

### Τιμή Επιστροφής

επιστρέφει true αν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline· διαφορετικά, false.

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

---

## Equals(object) {#equals_2}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


