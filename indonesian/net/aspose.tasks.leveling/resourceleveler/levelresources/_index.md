---
title: "ResourceLeveler.LevelResources"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceLeveler. Menyeimbangkan tugas untuk sumber daya yang ditentukan menggunakan opsi leveling yang ditentukan."
type: docs
weight: 30
url: /id/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Menyeimbangkan tugas untuk sumber daya yang ditentukan menggunakan opsi penyeimbangan yang ditentukan.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek untuk menerapkan leveling sumber daya. |
| opsi | LevelingOptions | Opsi yang menentukan cara menyeimbangkan sumber daya. |

### Nilai Kembali

Objek yang berisi hasil leveling sumber daya.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | jika parameter options bernilai null. |

## Contoh

Menampilkan cara menyeimbangkan sumber daya tertentu, menyesuaikan opsi penyeimbangan, dan memeriksa pesan algoritma penyeimbangan.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### Lihat Juga

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


