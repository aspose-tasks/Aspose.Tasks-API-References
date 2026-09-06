---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GraphicalIndicatorCriteria. Obtient le type de comparaison effectué entre la valeur des attributs étendus et les Valeurs qui sert de critère pour l'application de l'indicateur graphique. FilterComparisonType"
type: docs
weight: 40
url: /fr/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Obtient le type de comparaison effectué entre la valeur de l'attribut étendu et les Valeurs qui sert de critère pour l'application de l'indicateur graphique. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


