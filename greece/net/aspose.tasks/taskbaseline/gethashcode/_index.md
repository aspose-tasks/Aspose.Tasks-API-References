---
title: "TaskBaseline.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskBaseline method. Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης TaskBaseline"
type: docs
weight: 110
url: /el/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε τον κωδικό κατακερματισμού μιας βάσης εργασίας.

```csharp
var project = new Project();

// Δημιουργία TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Εμφάνιση διάρκειας baseline εργασίας
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// ο κωδικός κατακερματισμού ενός ημερολογίου είναι ίσος με τον αριθμό της βάσης
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Δείτε επίσης

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


