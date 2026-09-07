---
title: "Class FilterCriteria"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.FilterCriteria. Mendefinisikan kriteria yang harus dipenuhi oleh tugas atau sumber daya agar ditampilkan dalam tampilan MSP"
type: docs
weight: 630
url: /id/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Mendefinisikan kriteria yang harus dipenuhi oleh tugas atau sumber daya untuk ditampilkan dalam tampilan MSP.

```csharp
public class FilterCriteria
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Mendapatkan daftar baris `FilterCriteria` anak. Jika filter berisi lebih dari satu baris kriteria, maka efek operator And adalah kriteria untuk kedua baris harus dipenuhi agar tugas atau sumber daya ditampilkan sebagai hasil filter ini. Efek operator Or adalah kriteria untuk salah satu baris harus dipenuhi. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Mendapatkan atau mengatur sebuah [`Field`](./field/) untuk diubah. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Mendapatkan atau mengatur kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Mendapatkan atau mengatur jenis perbandingan antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Mendapatkan nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan dengan FieldName. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Mendapatkan apakah nilai sisi kanan FilterCriteria adalah referensi bidang, bukan nilai konstan. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Mengatur bidang yang nilainya akan dibandingkan dengan nilai bidang yang ditentukan oleh FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Mengembalikan representasi string dari instance kelas `FilterCriteria`. |

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


