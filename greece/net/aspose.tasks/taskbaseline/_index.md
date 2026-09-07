---
title: "Κλάση TaskBaseline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TaskBaseline. Αντιπροσωπεύει τη Βάση (Baseline) μιας Εργασίας"
type: docs
weight: 2370
url: /el/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Αντιπροσωπεύει το Baseline μιας Εργασίας.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Αρχικοποιεί μια νέα παρουσία της κλάσης `TaskBaseline`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Αποκτά ή ορίζει τον μοναδικό αριθμό μιας εγγραφής δεδομένων βάσης. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Αποκτά ή ορίζει το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Αποκτά ή ορίζει το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Αποκτά ή ορίζει το προβλεπόμενο κόστος ενός πόρου όταν η βάση αποθηκεύεται. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Λαμβάνει ή ορίζει τη προγραμματισμένη διάρκεια της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας εκτιμήθηκε. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Λαμβάνει ή ορίζει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Λαμβάνει ή ορίζει ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν πρόκειται για ενδιάμεση βάση αναφοράς. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Λαμβάνει ή ορίζει την προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία της TimephasedDataCollection για αυτό το αντικείμενο. Τα δεδομένα φάσης χρόνου που σχετίζονται με τη βάση αναφοράς της εργασίας. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Αποκτά ή ορίζει την εργασία που έχει ανατεθεί σε έναν πόρο όταν η βάση αποθηκεύεται. Το ποσό της ανατεθειμένης εργασίας σε έναν πόρο όταν η βάση αποθηκεύτηκε. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Υλοποίηση της διεπαφής IComparable. Συγκρίνει αυτήν την παρουσία με το καθορισμένο αντικείμενο Baseline. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | Υλοποίηση της διεπαφής IComparable. Συγκρίνει αυτήν την παρουσία με το καθορισμένο αντικείμενο Baseline. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης `TaskBaseline`. |

## Παραδείγματα

Δείχνει πώς να αποκτήσετε πρόσβαση σε πληροφορίες βάσης αναφοράς.

```csharp
var project = new Project();

// Δημιουργία TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Εμφάνιση διάρκειας βάσης αναφοράς εργασίας
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// τιμή που υποδεικνύει εάν πρόκειται για ενδιάμεση βάση αναφοράς
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// εκτύπωση δεδομένων φάσης χρόνου της βάσης αναφοράς εργασίας
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Δείτε επίσης

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


