---
title: "Enum HourLabelDisplay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.HourLabelDisplay. Menentukan bagaimana label jam ditampilkan"
type: docs
weight: 820
url: /id/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Menentukan bagaimana label jam ditampilkan.

```csharp
public enum HourLabelDisplay
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| H | `0` | "h" label. |
| Hr | `1` | "hr" label. |
| Hour | `2` | "hour(s)" label. |

## Contoh

Menampilkan cara mengatur label jam pada opsi tampilan proyek (kasus 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// atur bagaimana label jam ditampilkan
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


