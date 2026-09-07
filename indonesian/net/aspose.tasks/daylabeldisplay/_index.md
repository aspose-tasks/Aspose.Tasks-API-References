---
title: "Enum DayLabelDisplay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.DayLabelDisplay enum. Menentukan bagaimana label hari ditampilkan"
type: docs
weight: 440
url: /id/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Menentukan bagaimana label hari ditampilkan.

```csharp
public enum DayLabelDisplay
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| D | `0` | Mengatur daftar Hari di MS Project sebagai d. |
| Dy | `1` | Mengatur daftar Hari di MS Project sebagai dy. |
| Day | `2` | Mengatur daftar Hari di MS Project sebagai day. |

## Contoh

Menampilkan cara mengatur label hari dari opsi tampilan proyek (kasus 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// atur cara tampilan label hari
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


