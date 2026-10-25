---
title: "Enum EarnedValueMethodType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.EarnedValueMethodType enum. Menentukan metode yang digunakan untuk menghitung nilai yang diperoleh."
type: docs
weight: 480
url: /id/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Menentukan metode yang digunakan untuk menghitung nilai yang diperoleh.

```csharp
public enum EarnedValueMethodType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Bidang tidak didefinisikan dalam file proyek asli. |
| PercentComplete | `0` | Persentase selesai |
| PhysicalPercentComplete | `1` | Persentase fisik selesai |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara menentukan metode yang digunakan untuk menghitung nilai yang diperoleh (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// atur tipe metode nilai yang diperoleh menjadi 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// bekerja dengan proyek...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


