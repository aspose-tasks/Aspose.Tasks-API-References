---
title: "FilterCriteria.Operation"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα FilterCriteria. Λαμβάνει ή ορίζει το κριτήριο που καθορίζεται με το FieldName Test και το Value σχετίζεται με άλλα κριτήρια στο φίλτρο"
type: docs
weight: 40
url: /el/net/aspose.tasks/filtercriteria/operation/
---
## FilterCriteria.Operation property

Λαμβάνει ή ορίζει το κριτήριο που καθορίζεται με FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο.

```csharp
public FilterOperation Operation { get; set; }
```

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

* enum [FilterOperation](../../filteroperation/)
* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


