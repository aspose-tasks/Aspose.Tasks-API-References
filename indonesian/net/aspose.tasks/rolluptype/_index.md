---
title: "Enum RollupType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RollupType enum. Menentukan jenis rollup"
type: docs
weight: 1950
url: /id/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Menentukan jenis rollup.

```csharp
public enum RollupType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Null | `0` | Menunjukkan jenis rollup Null. |
| Maximum | `1` | Menunjukkan jenis rollup Maksimum. |
| Minimum | `2` | Menunjukkan jenis rollup Minimum. |
| Count | `3` | Menunjukkan jenis rollup Count. |
| Sum | `4` | Menunjukkan jenis rollup Sum. |
| Average | `5` | Menunjukkan jenis rollup Average. |
| AverageFirstSublevel | `6` | Menunjukkan jenis rollup Average First Sublevel. |
| CountFirstSublevel | `7` | Menunjukkan jenis rollup Count First Sublevel. |
| CountNonsummaries | `8` | Menunjukkan jenis rollup Count Non-Summaries. |

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


