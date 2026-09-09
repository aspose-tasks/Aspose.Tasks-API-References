---
title: "Enum MonthLabelDisplay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MonthLabelDisplay enum. Ay etiketinin nasıl görüntüleneceğini belirtir"
type: docs
weight: 1060
url: /tr/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Ay etiketinin nasıl görüntüleneceğini belirtir.

```csharp
public enum MonthLabelDisplay
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Mo | `0` | Aylar listesini MS Project'te mo olarak ayarlar. |
| Mon | `1` | Aylar listesini MS Project'te mon olarak ayarlar. |
| Month | `2` | Aylar listesini MS Project'te month olarak ayarlar. |

## Örnekler

Projenin görüntüleme seçeneklerinde ay etiketinin nasıl ayarlanacağını gösterir (durum 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ay etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


