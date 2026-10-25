---
title: "Enum DayLabelDisplay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.DayLabelDisplay enum. Gün etiketinin nasıl görüntüleneceğini belirtir"
type: docs
weight: 440
url: /tr/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Gün etiketinin nasıl görüntüleneceğini belirtir.

```csharp
public enum DayLabelDisplay
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| D | `0` | MS Project'teki Günler listesini d olarak ayarlar. |
| Dy | `1` | MS Project'teki Günler listesini dy olarak ayarlar. |
| Day | `2` | MS Project'teki Günler listesini day olarak ayarlar. |

## Örnekler

Projenin görüntüleme seçeneklerinde gün etiketini nasıl ayarlayacağınızı gösterir (durum 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// Gün etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


