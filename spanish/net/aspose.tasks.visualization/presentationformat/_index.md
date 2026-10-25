---
title: "Enumeración PresentationFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.PresentationFormat enum. Enumeración para el formato de presentación"
type: docs
weight: 3270
url: /es/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Enumeración para formato de presentación.

```csharp
public enum PresentationFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| GanttChart | `0` | Formato de presentación del diagrama de Gantt. |
| TaskUsage | `1` | Formato de presentación del uso de tareas. |
| ResourceUsage | `2` | Formato de presentación del uso de recursos. |
| ResourceSheet | `3` | Formato de presentación de la hoja de recursos. |
| TaskSheet | `4` | Formato de presentación de la hoja de tareas. |

## Ejemplos

Muestra cómo renderizar la vista de hoja de recursos.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Establezca el formato de presentación a Hoja de recursos
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


