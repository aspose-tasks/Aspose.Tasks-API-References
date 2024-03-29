---
title: FilterCriteria
second_title: Aspose.Tasks untuk Referensi .NET API
description: Menentukan kriteria yang harus dipenuhi tugas atau sumber daya untuk ditampilkan di tampilan MSP.
type: docs
weight: 630
url: /id/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Menentukan kriteria yang harus dipenuhi tugas atau sumber daya untuk ditampilkan di tampilan MSP.

```csharp
public class FilterCriteria
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Mendapat daftar anak`FilterCriteria` rows. Jika filter berisi lebih dari satu baris kriteria maka efek dari operator Dan adalah bahwa kriteria untuk kedua baris harus dipenuhi agar tugas atau sumber daya ditampilkan sebagai hasil dari filter ini. Efek dari Or operator adalah kriteria untuk satu atau baris lainnya harus dipenuhi. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Mendapat atau menyetel a[`Field`](./field/) untuk berubah. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Mendapat atau menyetel kriteria yang ditetapkan dengan NamaBidang, Tes, dan Nilai terkait dengan kriteria lain di filter. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Mendapat atau menyetel jenis perbandingan yang dibuat antara NamaBidang dan Nilai yang bertindak sebagai kriteria pemilihan untuk filter. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Mendapatkan nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan dengan NamaBidang. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Mengembalikan representasi string dari instance`FilterCriteria` kelas. |

### Lihat juga

* ruang nama [Aspose.Tasks](../../aspose.tasks/)
* perakitan [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
