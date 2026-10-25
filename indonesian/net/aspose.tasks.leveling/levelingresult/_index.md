---
title: "Class LevelingResult"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Leveling.LevelingResult. Mewakili hasil leveling sumber daya"
type: docs
weight: 960
url: /id/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Mewakili hasil perataan sumber daya.

```csharp
public sealed class LevelingResult
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [LevelingResult](levelingresult/)() | Menginisialisasi instance baru dari kelas `LevelingResult`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Mendapatkan sekumpulan tugas yang terpengaruh oleh leveling sumber daya. |

## Contoh

Menampilkan cara menyeimbangkan semua sumber daya proyek menggunakan opsi default.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### Lihat Juga

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


