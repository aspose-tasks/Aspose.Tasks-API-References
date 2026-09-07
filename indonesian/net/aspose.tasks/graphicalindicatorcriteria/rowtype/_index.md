---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GraphicalIndicatorCriteria. Mendapatkan nilai enum GraphicalIndicatorCriteriaType yang menunjukkan untuk baris mana indikator diterapkan"
type: docs
weight: 30
url: /id/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Mendapatkan nilai enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) yang menunjukkan untuk baris mana indikator diterapkan.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## Contoh

Menampilkan cara mengambil informasi indikator grafis.

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

### Lihat Juga

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


