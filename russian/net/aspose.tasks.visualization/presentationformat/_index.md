---
title: "Перечисление PresentationFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.PresentationFormat. Перечисление формата представления."
type: docs
weight: 3270
url: /ru/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Перечисление формата представления.

```csharp
public enum PresentationFormat
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| GanttChart | `0` | Формат представления диаграммы Ганта. |
| TaskUsage | `1` | Формат представления использования задач. |
| ResourceUsage | `2` | Формат представления использования ресурсов. |
| ResourceSheet | `3` | Формат представления листа ресурсов. |
| TaskSheet | `4` | Формат представления листа задач. |

## Примеры

Показывает, как отобразить представление листа ресурсов.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Установите формат представления в лист ресурсов.
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


