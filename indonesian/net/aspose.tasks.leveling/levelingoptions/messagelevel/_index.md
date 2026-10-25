---
title: "LevelingOptions.MessageLevel"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LevelingOptions. Mendapatkan atau mengatur tingkat pesan log yang dihasilkan oleh Aspose.Tasks selama penyeimbangan sumber daya"
type: docs
weight: 60
url: /id/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Mendapatkan atau mengatur tingkat pesan log yang dikeluarkan oleh Aspose.Tasks selama penyeimbangan sumber daya.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


