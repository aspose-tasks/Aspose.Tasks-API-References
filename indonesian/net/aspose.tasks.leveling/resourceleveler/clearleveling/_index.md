---
title: "ResourceLeveler.ClearLeveling"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceLeveler. Menghapus semua penundaan leveling yang sebelumnya ditambahkan ke proyek selama proses leveling sumber daya."
type: docs
weight: 10
url: /id/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Menghapus semua penundaan penyeimbangan yang sebelumnya ditambahkan ke proyek selama penyeimbangan sumber daya.

```csharp
public static void ClearLeveling(Project project)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek untuk menghapus leveling. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Menghapus semua penundaan penyeimbangan yang sebelumnya ditambahkan ke tugas yang ditentukan selama penyeimbangan sumber daya.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | IEnumerable`1 | Enumerable yang berisi tugas-tugas yang penundaan leveling-nya harus dihapus. |

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


