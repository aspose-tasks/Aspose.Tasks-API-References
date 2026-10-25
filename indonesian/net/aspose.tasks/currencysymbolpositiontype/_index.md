---
title: "Enum CurrencySymbolPositionType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.CurrencySymbolPositionType. Menentukan posisi simbol mata uang"
type: docs
weight: 370
url: /id/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Menentukan posisi simbol mata uang.

```csharp
public enum CurrencySymbolPositionType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan nilai undefined berarti bahwa bidang tidak didefinisikan dalam file proyek asli. |
| Before | `0` | Menunjukkan tipe posisi simbol mata uang Sebelum. |
| After | `1` | Menunjukkan tipe posisi simbol mata uang Setelah. |
| BeforeWithSpace | `2` | Menunjukkan tipe posisi simbol mata uang BeforeWithSpace. |
| AfterWithSpace | `3` | Menunjukkan tipe posisi simbol mata uang AfterWithSpace. |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara menentukan penempatan simbol mata uang (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// atur penempatan simbol mata uang
// Sebelum, tanpa spasi ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// bekerja dengan proyek...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


