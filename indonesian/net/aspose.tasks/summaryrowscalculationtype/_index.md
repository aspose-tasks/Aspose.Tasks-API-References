---
title: "Enum SummaryRowsCalculationType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.SummaryRowsCalculationType. Menentukan jenis perhitungan nilai atribut khusus untuk baris ringkasan."
type: docs
weight: 2310
url: /id/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

Menentukan jenis perhitungan nilai atribut khusus untuk baris ringkasan.

```csharp
public enum SummaryRowsCalculationType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Berarti nilai atribut khusus untuk baris ringkasan tidak dihitung. |
| Rollup | `1` | Berarti nilai atribut khusus untuk baris ringkasan dihitung menggunakan fungsi rollup yang didefinisikan dalam [`RollupType`](../extendedattributedefinition/rolluptype/). |
| UseFormula | `2` | Berarti nilai atribut khusus untuk baris ringkasan dihitung menggunakan formula yang didefinisikan dalam [`Formula`](../extendedattributedefinition/formula/). |

## Contoh

Menampilkan cara bekerja dengan tipe perhitungan dari definisi atribut yang diperluas.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// buat definisi atribut dengan tipe 'Formula' dimana nilai untuk tugas daun dan tugas ringkasan dihitung menggunakan formula.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// buat definisi atribut dimana nilai untuk tugas ringkasan dihitung menggunakan jenis rollup 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


