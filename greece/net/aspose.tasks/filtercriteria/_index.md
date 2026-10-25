---
title: "Κλάση FilterCriteria"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.FilterCriteria κλάση. Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP"
type: docs
weight: 630
url: /el/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP.

```csharp
public class FilterCriteria
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Λαμβάνει τη λίστα των θυγατρικών γραμμών `FilterCriteria`. Εάν το φίλτρο περιέχει περισσότερες από μία γραμμές κριτηρίων, τότε η επίδραση του τελεστή And είναι ότι τα κριτήρια και για τις δύο γραμμές πρέπει να ικανοποιηθούν ώστε η εργασία ή ο πόρος να εμφανιστούν ως αποτέλεσμα αυτού του φίλτρου. Η επίδραση του τελεστή Or είναι ότι τα κριτήρια για τη μία ή την άλλη γραμμή πρέπει να ικανοποιηθούν. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Λαμβάνει ή ορίζει ένα [`Field`](./field/) για αλλαγή. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Λαμβάνει ή ορίζει το κριτήριο που καθορίζεται με FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για το φίλτρο. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Λαμβάνει τις τιμές αντικειμένου για σύγκριση με την τιμή του πεδίου που καθορίζεται με FieldName. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Λαμβάνει αν η δεξιά τιμή του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Ορίζει το πεδίο του οποίου η τιμή θα συγκριθεί με την τιμή του πεδίου που καθορίζεται από FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Επιστρέφει την αναπαράσταση σε συμβολοσειρά της παρουσίας της κλάσης `FilterCriteria`. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα κριτήρια φίλτρου εργασιών.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// Εκτύπωση κριτηρίων φίλτρου ως συμβολοσειρά
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


