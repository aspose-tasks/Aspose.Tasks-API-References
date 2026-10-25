---
title: "Class LevelingResult"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Leveling.LevelingResult sınıfı. Kaynak dengelemesinin sonuçlarını temsil eder."
type: docs
weight: 960
url: /tr/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Kaynak dengelemesinin sonuçlarını temsil eder.

```csharp
public sealed class LevelingResult
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LevelingResult](levelingresult/)() | Yeni bir `LevelingResult` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Kaynak dengelemesinden etkilenen görevlerin bir kümesini alır. |

## Örnekler

Varsayılan seçenekleri kullanarak projenin tüm kaynaklarını nasıl dengeleyeceğinizi gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


