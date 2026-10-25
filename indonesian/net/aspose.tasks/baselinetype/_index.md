---
title: "Enum BaselineType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.BaselineType. Menentukan jenis baseline yang digunakan untuk menghitung nilai Variance."
type: docs
weight: 130
url: /id/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Menentukan tipe baseline yang digunakan untuk menghitung nilai Variansi.

```csharp
public enum BaselineType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan bahwa bidang tidak didefinisikan dalam file proyek asli. |
| Baseline | `0` | Menunjukkan jenis Baseline. |
| Baseline1 | `1` | Menunjukkan jenis Baseline1. |
| Baseline2 | `2` | Menunjukkan jenis Baseline2. |
| Baseline3 | `3` | Menunjukkan jenis Baseline3. |
| Baseline4 | `4` | Menunjukkan jenis Baseline4. |
| Baseline5 | `5` | Menunjukkan jenis Baseline5. |
| Baseline6 | `6` | Menunjukkan jenis Baseline6. |
| Baseline7 | `7` | Menunjukkan jenis Baseline7. |
| Baseline8 | `8` | Menunjukkan jenis Baseline8. |
| Baseline9 | `9` | Menunjukkan jenis Baseline9. |
| Baseline10 | `10` | Menunjukkan jenis Baseline10. |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara mengatur baseline untuk proyek (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Menyimpan bidang baseline ke baseline yang ditentukan untuk seluruh proyek.
project.SetBaseline(BaselineType.Baseline);
// Bekerja dengan baseline proyek...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


