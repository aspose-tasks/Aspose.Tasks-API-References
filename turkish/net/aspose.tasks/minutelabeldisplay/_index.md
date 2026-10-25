---
title: "Enum MinuteLabelDisplay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MinuteLabelDisplay enum. Dakika etiketinin nasıl görüntüleneceğini belirtir."
type: docs
weight: 1030
url: /tr/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Dakika etiketinin nasıl görüntüleneceğini belirtir.

```csharp
public enum MinuteLabelDisplay
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| M | `0` | MS Project'teki Dakikalar listesini m olarak ayarlar. |
| Min | `1` | MS Project'teki Dakikalar listesini min olarak ayarlar. |
| Minute | `2` | MS Project'teki Dakikalar listesini minute olarak ayarlar. |

## Örnekler

Projenin görüntüleme seçeneklerinin dakika etiketinin nasıl ayarlanacağını gösterir (durum 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// dakika etiketinin nasıl görüntüleneceğini ayarlar
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


