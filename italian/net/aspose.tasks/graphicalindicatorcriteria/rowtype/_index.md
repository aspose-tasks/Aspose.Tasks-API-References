---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GraphicalIndicatorCriteria. Ottiene il valore dell'enumerazione GraphicalIndicatorCriteriaType che indica per quali righe l'indicatore è applicato"
type: docs
weight: 30
url: /it/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Ottiene il valore dell'enumerazione [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) che indica per quali righe l'indicatore è applicato.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## Esempi

Mostra come recuperare le informazioni degli indicatori grafici.

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

### Vedi anche

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


