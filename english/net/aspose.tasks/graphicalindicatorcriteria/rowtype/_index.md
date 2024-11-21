---
title: GraphicalIndicatorCriteria.RowType
second_title: Aspose.Tasks for .NET API Reference
description: GraphicalIndicatorCriteria property. Gets the value of GraphicalIndicatorCriteriaType enum which denotes for which rows the indicator is applied
type: docs
weight: 30
url: /net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Gets the value of [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum which denotes for which rows the indicator is applied.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## Examples

Shows how to retrieve graphical indicators info.

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

### See Also

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


