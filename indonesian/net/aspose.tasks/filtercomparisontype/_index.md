---
title: "Enum FilterComparisonType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.FilterComparisonType enum. Jenis perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter atau indikator grafis."
type: docs
weight: 620
url: /id/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Tipe perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter atau indikator grafis.

```csharp
public enum FilterComparisonType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Equals | `6` | Nilai Field sama dengan Value. |
| DoesNotEqual | `7` | Nilai Field tidak sama dengan Value. |
| IsGreaterThan | `2` | Nilai Field lebih besar dari Value. |
| IsGreaterThanOrEqualTo | `4` | Nilai Field lebih besar dari atau sama dengan Value. |
| IsLessThan | `3` | Nilai Field lebih kecil dari Value. |
| IsLessThanOrEqualTo | `5` | Nilai Field lebih kecil dari atau sama dengan Value. |
| IsWithin | `1` | Nilai Field berada dalam Value. |
| IsNotWithin | `9` | Nilai Field tidak berada dalam Value. |
| Contains | `8` | Nilai Field mengandung Value. |
| DoesNotContain | `10` | Nilai Field tidak mengandung Value. |
| ContainsExactly | `11` | Nilai Field secara tepat mengandung Value. |
| IsOneOf | `12` | Nilai Field sama dengan salah satu Values yang ditentukan. Digunakan dalam AutoFilters. |
| Undefined | `0` | Nilai tidak terdefinisi. |
| IsAnyValue | `255` | Kondisi 'Is any value'. Berlaku untuk indikator grafis. |

## Contoh

Menampilkan cara membaca kriteria filter tugas.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// kriteria filter cetak sebagai string
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


