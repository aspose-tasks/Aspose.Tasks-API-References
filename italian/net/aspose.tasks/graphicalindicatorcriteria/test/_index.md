---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GraphicalIndicatorCriteria. Ottiene il tipo di confronto effettuato tra il valore degli attributi estesi e i Valori che fungono da criterio per l'applicazione dell'indicatore grafico. FilterComparisonType"
type: docs
weight: 40
url: /it/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Ottiene il tipo di confronto effettuato tra il valore dell'attributo esteso e i Valori che fungono da criterio per l'applicazione dell'indicatore grafico. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


