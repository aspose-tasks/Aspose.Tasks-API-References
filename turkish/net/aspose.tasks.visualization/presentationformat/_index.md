---
title: "Enum PresentationFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PresentationFormat enum. Sunum formatı için bir enum"
type: docs
weight: 3270
url: /tr/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Sunum biçimi için numaralandırma.

```csharp
public enum PresentationFormat
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| GanttChart | `0` | Gantt Şeması sunum formatı. |
| TaskUsage | `1` | Görev kullanımı sunum formatı. |
| ResourceUsage | `2` | Kaynak kullanımı sunum formatı. |
| ResourceSheet | `3` | Kaynak sayfası sunum formatı. |
| TaskSheet | `4` | Görev sayfası sunum formatı. |

## Örnekler

Kaynak sayfası görünümünün nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Sunum Formatını Kaynak Sayfası olarak ayarla
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


