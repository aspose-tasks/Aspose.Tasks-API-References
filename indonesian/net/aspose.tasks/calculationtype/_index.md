---
title: "Enum CalculationType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.CalculationType. Menentukan jenis perhitungan nilai atribut khusus"
type: docs
weight: 220
url: /id/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Menentukan tipe perhitungan nilai atribut khusus.

```csharp
public enum CalculationType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Berarti atribut tambahan tidak memiliki tabel pencarian rumus dan hanya menyimpan nilai yang ditetapkan oleh pengguna. |
| Lookup | `1` | Berarti nilai atribut tambahan dibatasi pada nilai-nilai dari tabel pencarian. |
| Formula | `2` | Berarti nilai atribut tambahan dihitung menggunakan rumus yang didefinisikan dalam [`Formula`](../extendedattributedefinition/formula/). |

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


