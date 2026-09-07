---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GraphicalIndicatorCriteria. Mendapatkan nilai kedua yang digunakan untuk menguji nilai atribut yang diperluas dalam kasus tipe perbandingan IsWithin dan IsNotWithin"
type: docs
weight: 60
url: /id/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

Mendapatkan nilai kedua yang digunakan untuk menguji nilai atribut yang diperluas dalam kasus tipe perbandingan 'IsWithin' dan 'IsNotWithin'.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


