---
title: "Enumeración GridlineType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Visualization.GridlineType. Tipo de línea de cuadrícula."
type: docs
weight: 3110
url: /es/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Tipo de línea de cuadrícula.

```csharp
public enum GridlineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| GanttRow | `0` | Indica la línea de cuadrícula de una fila de Gantt. |
| TopTierColumn | `1` | Indica la línea de cuadrícula de la columna de nivel superior. |
| BottomTierColumn | `2` | Indica la línea de cuadrícula de la columna de nivel inferior. |
| SheetRow | `3` | Indica la línea de cuadrícula de una fila de hoja. |
| SheetColumn | `4` | Indica la línea de cuadrícula de una columna de hoja. |
| UsageRow | `5` | Indica la línea de cuadrícula de una fila de uso. |
| UsageColumn | `6` | Indica la línea de cuadrícula de una columna de uso. |
| GanttTitleVertical | `7` | Indica el tipo de línea de cuadrícula vertical del título de Gantt. |
| GanttTitleHorizontal | `8` | Indica el tipo de línea de cuadrícula horizontal del título de Gantt. |
| BarRows | `9` | Indica el tipo de línea de cuadrícula de filas de barra. |
| GanttProjectStart | `10` | Indica el tipo de línea de cuadrícula de inicio del proyecto Gantt. |
| GanttProjectFinish | `11` | Indica el tipo de línea de cuadrícula de final del proyecto Gantt. |
| GanttStatusDate | `12` | Indica el tipo de línea de cuadrícula de la fecha de estado de Gantt. |
| GanttCurrentDate | `13` | Indica el tipo de línea de cuadrícula de la fecha actual de Gantt. |
| GanttPageBreaks | `14` | Indica el tipo de línea de cuadrícula de los saltos de página de Gantt. |
| MiddleTierColumn | `15` | Indica la línea de cuadrícula del tipo de línea de cuadrícula de la columna de nivel intermedio. |

## Ejemplos

Muestra cómo trabajar con líneas de cuadrícula al guardar en formatos visuales.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // establece el tipo de línea de cuadrícula (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // establece el <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> de una línea de cuadrícula
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


