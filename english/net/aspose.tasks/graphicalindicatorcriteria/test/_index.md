---
title: GraphicalIndicatorCriteria.Test
second_title: Aspose.Tasks for .NET API Reference
description: GraphicalIndicatorCriteria property. Gets the type of comparison made between extended attributes value and Values that acts as a criteria for the application of the graphical indicator. FilterComparisonType
type: docs
weight: 40
url: /net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Gets the type of comparison made between extended attribute's value and Values that acts as a criteria for the application of the graphical indicator. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


