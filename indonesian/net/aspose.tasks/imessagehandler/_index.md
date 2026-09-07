---
title: "Antarmuka IMessageHandler"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Antarmuka Aspose.Tasks.IMessageHandler. Mewakili callback hasil leveling sumber daya"
type: docs
weight: 880
url: /id/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Mewakili callback hasil penyeimbangan sumber daya.

```csharp
public interface IMessageHandler
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks memanggil metode ini ketika mengeluarkan pesan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


