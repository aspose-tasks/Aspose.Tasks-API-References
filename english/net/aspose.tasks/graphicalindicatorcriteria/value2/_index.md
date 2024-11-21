---
title: GraphicalIndicatorCriteria.Value2
second_title: Aspose.Tasks for .NET API Reference
description: GraphicalIndicatorCriteria property. Gets the second value used to test extended attributes value in case of IsWithin and IsNotWithin comparison types
type: docs
weight: 60
url: /net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

Gets the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


