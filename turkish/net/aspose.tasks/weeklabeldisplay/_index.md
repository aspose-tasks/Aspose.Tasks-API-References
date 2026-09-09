---
title: "Enum WeekLabelDisplay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WeekLabelDisplay enum. Haftanın etiketi nasıl görüntüleneceğini belirtir"
type: docs
weight: 3560
url: /tr/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Hafta etiketinin nasıl görüntüleneceğini belirtir.

```csharp
public enum WeekLabelDisplay
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| W | `0` | "w" etiketi. |
| Wk | `1` | "wk" etiketi. |
| Week | `2` | "week" etiketi. |

## Örnekler

Projenin görüntüleme seçeneklerinde hafta etiketini nasıl ayarlayacağınızı gösterir (durum 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// Hafta etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


