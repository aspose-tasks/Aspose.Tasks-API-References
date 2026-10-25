---
title: "Sınıf LevelingOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Leveling.LevelingOptions sınıfı. Kaynak dengelemesinin parametrelerini belirtmeye olanak tanır"
type: docs
weight: 940
url: /tr/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Kaynak dengelemesinin parametrelerini belirtmeye izin verir.

```csharp
public sealed class LevelingOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | `LevelingOptions` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Bir proje dengeleme işlemini iptal etmek için kullanılabilecek bir token alır veya ayarlar. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Dengeleme dönemi bitiş tarihini alır veya ayarlar. Varsayılan değer projenin bitiş tarihidir. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Aşırı tahsisata sahip görevlerin dengeleme algoritması tarafından geciktirileceği sıralamayı alır. Aşırı tahsise neden olan ve geciktirilebilecek görevler belirlendikten sonra, hangi görevin önce geciktirileceğini belirlemek için belirtilen sıra kullanılır. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Aspose.Tasks tarafından kaynak dengelemesi sırasında üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını alır veya ayarlar. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Aspose.Tasks tarafından kaynak dengelemesi sırasında yayımlanan günlük mesajlarının seviyesini alır veya ayarlar. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Dengelenecek kaynakların listesini alır veya ayarlar. Null ayarlanırsa, projenin tüm kaynakları dengelenecektir. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Dengeleme dönemi başlangıç tarihini alır veya ayarlar. Varsayılan değer projenin başlangıç tarihidir. |

## Örnekler

Belirli bir kaynağı dengelemeyi, dengeleme seçeneklerini özelleştirmeyi ve dengeleme algoritması mesajlarını incelemeyi gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


