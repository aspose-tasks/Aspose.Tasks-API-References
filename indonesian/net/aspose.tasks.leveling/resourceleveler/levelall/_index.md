---
title: "ResourceLeveler.LevelAll"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceLeveler. Menyeimbangkan tugas untuk semua sumber daya proyek menggunakan opsi leveling default."
type: docs
weight: 20
url: /id/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Menyeimbangkan tugas untuk semua sumber daya proyek menggunakan opsi penyeimbangan default.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek untuk menerapkan leveling sumber daya. |

### Nilai Kembali

Objek yang berisi hasil leveling sumber daya.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


