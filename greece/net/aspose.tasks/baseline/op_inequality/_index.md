---
title: "Baseline.op_Inequality"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Baseline. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο"
type: docs
weight: 130
url: /el/net/aspose.tasks/baseline/op_inequality/
---
## Baseline Inequality operator

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public static bool operator !=(Baseline a, Baseline b)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| α | Baseline | Το πρώτο baseline. |
| β | Baseline | Το δεύτερο baseline. |

### Τιμή Επιστροφής

μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο

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

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


