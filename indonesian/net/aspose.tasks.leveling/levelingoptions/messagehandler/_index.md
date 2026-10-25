---
title: "LevelingOptions.MessageHandler"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LevelingOptions. Mendapatkan atau mengatur callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama penyeimbangan sumber daya"
type: docs
weight: 50
url: /id/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Mendapatkan atau mengatur callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama penyeimbangan sumber daya.

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


