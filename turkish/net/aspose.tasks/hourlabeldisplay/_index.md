---
title: "Enum HourLabelDisplay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.HourLabelDisplay enum. Saat etiketinin nasıl görüntüleneceğini belirtir"
type: docs
weight: 820
url: /tr/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Saat etiketinin nasıl görüntüleneceğini belirtir.

```csharp
public enum HourLabelDisplay
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| H | `0` | "h" etiketi. |
| Hr | `1` | "hr" etiketi. |
| Hour | `2` | "hour(s)" etiketi. |

## Örnekler

Projenin görüntüleme seçeneklerinde saat etiketinin nasıl ayarlanacağını gösterir (durum 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// saat etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


