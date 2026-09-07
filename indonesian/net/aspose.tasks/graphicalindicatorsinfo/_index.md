---
title: "Kelas GraphicalIndicatorsInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.GraphicalIndicatorsInfo. Mewakili definisi indikator grafis yang terkait dengan atribut ekstended"
type: docs
weight: 760
url: /id/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Mewakili definisi indikator grafis yang terkait dengan atribut tambahan.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Menginisialisasi instance baru dari tipe `GraphicalIndicatorsInfo`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Mendapatkan daftar kriteria indikator grafis. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Mendapatkan atau mengatur flag yang menunjukkan apakah baris ringkasan proyek mewarisi kriteria dari baris ringkasan. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Mendapatkan atau mengatur flag yang menunjukkan apakah nilai data untuk bidang harus ditampilkan dalam tooltip. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Mendapatkan atau mengatur flag yang menunjukkan apakah baris ringkasan mewarisi kriteria dari baris non-ringkasan. |

## Contoh

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


