---
title: "Project.DisplayOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan sebuah instance dari kelas ProjectDisplayOptions"
type: docs
weight: 380
url: /id/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Mendapatkan sebuah instance dari kelas `[`ProjectDisplayOptions`](../../projectdisplayoptions/)`.

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Contoh

Menampilkan cara menyesuaikan opsi tampilan proyek.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Mengatur nilai yang menunjukkan apakah menampilkan peringatan ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual.
// Opsi ini tersedia untuk versi Project 2010 dan yang lebih baru.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Lihat Juga

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


