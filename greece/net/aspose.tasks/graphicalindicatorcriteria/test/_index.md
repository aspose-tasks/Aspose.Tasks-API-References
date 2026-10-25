---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GraphicalIndicatorCriteria. Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ της τιμής των εκτεταμένων χαρακτηριστικών και των τιμών που λειτουργούν ως κριτήριο για την εφαρμογή του γραφικού δείκτη. FilterComparisonType"
type: docs
weight: 40
url: /el/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ της τιμής του εκτεταμένου χαρακτηριστικού και των τιμών που λειτουργούν ως κριτήριο για την εφαρμογή του γραφικού δείκτη. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
```

## Παραδείγματα

Δείχνει πώς να ανακτήσετε πληροφορίες γραφικών δεικτών.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

### Δείτε επίσης

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


