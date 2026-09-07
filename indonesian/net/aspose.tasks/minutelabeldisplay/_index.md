---
title: "Enum MinuteLabelDisplay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.MinuteLabelDisplay. Menentukan cara tampilan label menit."
type: docs
weight: 1030
url: /id/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Menentukan bagaimana label menit ditampilkan.

```csharp
public enum MinuteLabelDisplay
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| M | `0` | Mengatur daftar Menit di MS Project sebagai m. |
| Min | `1` | Mengatur daftar Menit di MS Project sebagai min. |
| Minute | `2` | Mengatur daftar Menit di MS Project sebagai minute. |

## Contoh

Menampilkan cara mengatur label menit pada opsi tampilan proyek (kasus 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// atur bagaimana label menit ditampilkan
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


