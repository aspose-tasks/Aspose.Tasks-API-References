---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GraphicalIndicatorCriteria. Ottiene il secondo valore usato per testare il valore degli attributi estesi nei casi di tipi di confronto IsWithin e IsNotWithin"
type: docs
weight: 60
url: /it/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

Ottiene il secondo valore usato per testare il valore dell'attributo esteso nel caso dei tipi di confronto 'IsWithin' e 'IsNotWithin'.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


