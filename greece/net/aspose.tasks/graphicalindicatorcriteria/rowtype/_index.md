---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GraphicalIndicatorCriteria. Λαμβάνει την τιμή του enum GraphicalIndicatorCriteriaType που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης."
type: docs
weight: 30
url: /el/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Λαμβάνει την τιμή του enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
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

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


