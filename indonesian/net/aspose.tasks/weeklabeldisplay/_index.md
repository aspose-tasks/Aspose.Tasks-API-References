---
title: "Enum WeekLabelDisplay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.WeekLabelDisplay enum. Menentukan bagaimana label minggu ditampilkan"
type: docs
weight: 3560
url: /id/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Menentukan bagaimana label minggu ditampilkan.

```csharp
public enum WeekLabelDisplay
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| W | `0` | "w" label. |
| Wk | `1` | "wk" label. |
| Week | `2` | "week" label. |

## Contoh

Menampilkan cara mengatur label minggu dari opsi tampilan proyek (kasus 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// atur cara tampilan label minggu
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


