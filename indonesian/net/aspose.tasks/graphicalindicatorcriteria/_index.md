---
title: "Kelas GraphicalIndicatorCriteria"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.GraphicalIndicatorCriteria. Mewakili satu kriteria indikator grafis yang terkait dengan atribut ekstensi"
type: docs
weight: 730
url: /id/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Mewakili satu kriteria indikator grafis yang terkait dengan atribut tambahan.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Menginisialisasi instance baru dari tipe `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Menginisialisasi instance baru dari tipe `GraphicalIndicatorCriteria`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Mendapatkan indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Mendapatkan nilai enum [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) yang menunjukkan untuk baris mana indikator diterapkan. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Mendapatkan tipe perbandingan yang dibuat antara nilai atribut ekstensi dan Nilai yang berfungsi sebagai kriteria untuk penerapan indikator grafis. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Mendapatkan nilai yang digunakan untuk menguji nilai atribut yang diperluas. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Mendapatkan nilai kedua yang digunakan untuk menguji nilai atribut yang diperluas dalam kasus tipe perbandingan 'IsWithin' dan 'IsNotWithin'. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Mengembalikan representasi string dari instance kelas `GraphicalIndicatorCriteria`. |

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

Menampilkan cara menyiapkan indikator grafis untuk atribut yang diperluas.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// Kriteria 'IsWithin' memerlukan 2 nilai.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// Kriteria 'IsAnyValue' tidak memerlukan nilai.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


