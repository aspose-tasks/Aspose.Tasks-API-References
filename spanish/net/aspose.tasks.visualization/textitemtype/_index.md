---
title: "Enumeración TextItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Visualization.TextItemType. Tipo de elemento para cambiar un estilo de texto"
type: docs
weight: 3410
url: /es/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Tipo de elemento para cambiar un estilo de texto.

```csharp
public enum TextItemType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| RowColumnTitles | `0` | Títulos de filas y columnas. |
| CriticalTasks | `1` | Tareas críticas. |
| NoncriticalTasks | `2` | Tareas no críticas. |
| MilestoneTasks | `3` | Tareas de hito. |
| InactiveTasks | `4` | Tareas inactivas. |
| SummaryTasks | `5` | Tareas de resumen. |
| AssignmentRow | `6` | Fila de asignación. |
| TopTimescaleTier | `7` | Nivel superior de escala de tiempo. |
| BottomTimescaleTier | `8` | Nivel inferior de escala de tiempo. |
| MiddleTimescaleTier | `9` | Nivel medio de escala de tiempo. |
| Resources | `10` | Hoja de recursos. |
| OverallocatedResources | `11` | Recursos sobreasignados. |
| TaskFilterHighlight | `12` | Elemento de texto de resaltado de filtro de tarea. |
| BarTextBottom | `13` | Elemento de texto inferior de barra. |
| BarTextInside | `14` | Elemento de texto interior de barra. |
| BarTextLeft | `15` | Elemento de texto izquierdo de barra. |
| BarTextRight | `16` | Elemento de texto derecho de barra. |
| BarTextTop | `17` | Elemento de texto superior de barra. |
| MarkedTasks | `18` | Elemento de texto de tarea marcada. |
| ProjectSummary | `19` | Elemento de texto de tarea de resumen del proyecto. |
| ExternalTasks | `20` | Elemento de texto de tareas externas. |
| Allocated | `21` | Elemento de texto asignado. |
| ChangedCells | `22` | Celdas modificadas. |

## Ejemplos

Muestra cómo trabajar con tipos de elementos de texto.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


