---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GraphicalIndicatorCriteria. Obtient la valeur de l'énumération GraphicalIndicatorCriteriaType qui indique pour quelles lignes l'indicateur est appliqué"
type: docs
weight: 30
url: /fr/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Obtient la valeur de l'énumération [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) qui indique pour quelles lignes l'indicateur est appliqué.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## Exemples

Montre comment récupérer les informations des indicateurs graphiques.

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

### Voir aussi

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


