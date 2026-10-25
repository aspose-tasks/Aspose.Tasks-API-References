---
title: "TaskLink.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskLink μέθοδος. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο"
type: docs
weight: 90
url: /el/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public bool Equals(TaskLink other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | TaskLink | Η καθορισμένη παρουσία της κλάσης [`TaskLink`](../) για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των συνδέσεων εργασιών.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Η ισότητα των συνδέσεων εργασιών βασίζεται στις προγενέστερες και επόμενες εργασίες.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Δείτε επίσης

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των συνδέσεων εργασιών.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Η ισότητα των συνδέσεων εργασιών βασίζεται στις προγενέστερες και επόμενες εργασίες.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Δείτε επίσης

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


