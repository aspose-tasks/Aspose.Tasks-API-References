---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "GraphicalIndicatorCriteria свойство. Получает значение перечисления GraphicalIndicatorCriteriaType, которое указывает, для каких строк применяется индикатор."
type: docs
weight: 30
url: /ru/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Получает значение перечисления [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/), которое указывает, для каких строк применяется индикатор.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## Примеры

Показывает, как получить информацию о графических индикаторах.

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

### См. также

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


