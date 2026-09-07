---
title: "Enum FilterComparisonType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.FilterComparisonType enum. Ο τύπος σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για ένα φίλτρο ή γραφικό δείκτη"
type: docs
weight: 620
url: /el/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Ο τύπος σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για ένα φίλτρο ή γραφικό δείκτη.

```csharp
public enum FilterComparisonType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Equals | `6` | Η τιμή του Field είναι ίση με Value. |
| DoesNotEqual | `7` | Η τιμή του Field δεν είναι ίση με Value. |
| IsGreaterThan | `2` | Η τιμή του Field είναι μεγαλύτερη από Value. |
| IsGreaterThanOrEqualTo | `4` | Η τιμή του Field είναι μεγαλύτερη ή ίση με Value. |
| IsLessThan | `3` | Η τιμή του Field είναι μικρότερη από Value. |
| IsLessThanOrEqualTo | `5` | Η τιμή του Field είναι μικρότερη ή ίση με Value. |
| IsWithin | `1` | Η τιμή του Field βρίσκεται εντός Value. |
| IsNotWithin | `9` | Η τιμή του Field δεν βρίσκεται εντός Value. |
| Contains | `8` | Η τιμή του Field περιέχει Value. |
| DoesNotContain | `10` | Η τιμή του Field δεν περιέχει Value. |
| ContainsExactly | `11` | Η τιμή του Field περιέχει ακριβώς Value. |
| IsOneOf | `12` | Η τιμή του Field ισούται με μία από τις καθορισμένες Values. Χρησιμοποιείται στα AutoFilters. |
| Undefined | `0` | Απροσδιόριστη τιμή. |
| IsAnyValue | `255` | Συνθήκη 'Is any value'. Εφαρμόσιμη σε γραφικούς δείκτες. |

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


