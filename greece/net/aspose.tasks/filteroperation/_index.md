---
title: "Απαρίθμηση FilterOperation"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.FilterOperation. Καθορίζει πώς το κριτήριο που ορίζεται με FieldName, FilterComparisonType και Value σχετίζεται με άλλα κριτήρια στο φίλτρο."
type: docs
weight: 640
url: /el/net/aspose.tasks/filteroperation/
---
## FilterOperation enumeration

Καθορίζει πώς το κριτήριο που καθορίζεται με τα FieldName, FilterComparisonType και Value σχετίζεται με άλλα κριτήρια στο φίλτρο.

```csharp
public enum FilterOperation
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `0` | Απροσδιόριστο. |
| And | `1` | Τελεστής AND. |
| Or | `2` | Τελεστής OR. |

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


