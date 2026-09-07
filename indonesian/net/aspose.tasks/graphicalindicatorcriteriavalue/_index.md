---
title: "Kelas GraphicalIndicatorCriteriaValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.GraphicalIndicatorCriteriaValue. Mewakili nilai yang digunakan dalam pemeriksaan kondisi kriteria indikator grafis."
type: docs
weight: 750
url: /id/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

Mewakili nilai yang digunakan dalam pemeriksaan kondisi kriteria indikator grafis.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | Membuat instance kelas GraphicalIndicatorCriteriaValue dengan nilai flag (bool) konstan. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | Membuat instance kelas GraphicalIndicatorCriteriaValue dengan nilai DateTime konstan. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | Membuat instance kelas GraphicalIndicatorCriteriaValue dengan nilai desimal konstan. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | Membuat instance kelas GraphicalIndicatorCriteriaValue dengan nilai Duration konstan. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | Membuat instance kelas GraphicalIndicatorCriteriaValue dengan nilai string konstan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | Mendapatkan apakah instance saat ini adalah tautan bidang (mewakili nilai sebuah bidang). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | Mendapatkan konstanta dasar dari nilai Field. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | Membuat sebuah instance dari kelas GraphicalIndicatorCriteriaValue yang mewakili nilai dari field MS Project yang ditentukan. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | Mengembalikan string yang mewakili objek saat ini. |

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


