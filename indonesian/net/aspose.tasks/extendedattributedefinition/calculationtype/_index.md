---
title: "ExtendedAttributeDefinition.CalculationType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttributeDefinition. Mendapatkan atau mengatur tipe perhitungan nilai atribut khusus."
type: docs
weight: 80
url: /id/net/aspose.tasks/extendedattributedefinition/calculationtype/
---
## ExtendedAttributeDefinition.CalculationType property

Mendapatkan atau mengatur tipe perhitungan nilai atribut khusus.

```csharp
public CalculationType CalculationType { get; set; }
```

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

* enum [CalculationType](../../calculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


