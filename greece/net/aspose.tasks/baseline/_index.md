---
title: "Κλάση Baseline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Baseline κλάση. Αντιπροσωπεύει τις τιμές baseline ενός πόρου."
type: docs
weight: 110
url: /el/net/aspose.tasks/baseline/
---
## Baseline class

Αντιπροσωπεύει τις τιμές βάσης ενός πόρου.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Baseline](baseline/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Αποκτά ή ορίζει τον μοναδικό αριθμό μιας εγγραφής δεδομένων βάσης. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Αποκτά ή ορίζει το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Αποκτά ή ορίζει το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Αποκτά ή ορίζει το προβλεπόμενο κόστος ενός πόρου όταν η βάση αποθηκεύεται. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Αποκτά ή ορίζει την εργασία που έχει ανατεθεί σε έναν πόρο όταν η βάση αποθηκεύεται. Το ποσό της ανατεθειμένης εργασίας σε έναν πόρο όταν η βάση αποθηκεύτηκε. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Υλοποίηση της διεπαφής IComparable. Συγκρίνει αυτήν την παρουσία με το καθορισμένο αντικείμενο Baseline. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το baseline. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις βάσεις των αναθέσεων.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Οι βάσεις των αναθέσεων ορίζονται όταν ορίζεται η βάση σε ολόκληρο το έργο.
project.SetBaseline(BaselineType.Baseline);

// διαβάστε πληροφορίες βάσης ανάθεσης
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// ελέγξτε την ισότητα της βάσης
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// Οι βάσεις μπορούν να συγκριθούν χρησιμοποιώντας τις υπερφορτώσεις της μεθόδου 'Equals'
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// ή χρησιμοποιώντας υπερφορτωμένη αριθμητική λειτουργία
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// Ο κωδικός κατακερματισμού της βάσης βασίζεται στον αριθμό της βάσης
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


