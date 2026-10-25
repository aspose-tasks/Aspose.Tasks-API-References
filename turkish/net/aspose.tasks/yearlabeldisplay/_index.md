---
title: "Enum YearLabelDisplay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.YearLabelDisplay enum. Yıl etiketinin nasıl görüntüleneceğini belirtir."
type: docs
weight: 3680
url: /tr/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Yıl etiketinin nasıl görüntüleneceğini belirtir.

```csharp
public enum YearLabelDisplay
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Y | `0` | MS Project'teki Yıllar listesini mo olarak ayarlar. |
| Yr | `1` | MS Project'teki Yıllar listesini mon olarak ayarlar. |
| Year | `2` | MS Project'teki Yıllar listesini ay olarak ayarlar. |

## Örnekler

Projenin görüntüleme seçeneklerinde yıl etiketinin nasıl ayarlanacağını gösterir (durum 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// yıl etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


